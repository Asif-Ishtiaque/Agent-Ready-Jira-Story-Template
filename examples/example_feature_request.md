# FEAT-801 - Agent-Ready User Story: Header Theme Selector Toggle

## 1. Context & Objectives
*   **Persona / Role**: As a Frontend developer agent...
*   **Goal**: I want to add a theme toggle button (Sun/Moon icons) to the header.
*   **Business Value**: So that users can switch between Light and Dark mode, improving readability and user experience.
*   **Problem Statement**: The website has fully implemented dark mode utility classes in tailwind/CSS, but there is no user-facing UI control in the Header component to switch between themes.

## 2. Technical Scope & System Boundary
*   **Target Components**: Header and Navigation
*   **Target Files**:
    - `src/components/Header.jsx`
    - `src/context/ThemeContext.jsx` (already exists, exports `useTheme` hook with `{ theme, toggleTheme }`)
*   **System Dependencies**: Integrates with the pre-existing `ThemeContext`.

## 3. Acceptance Criteria (Gherkin Format)

### Scenario 1: Initial state and toggling to dark mode
*   **Given** the user is viewing the page with the default "light" theme
*   **When** they click the theme toggle button in the Header
*   **Then** the theme should switch to "dark"
*   **And** the document body or root HTML element should receive the `dark` class
*   **And** the toggle button icon should change from a Sun icon (representing light theme) to a Moon icon (representing dark theme).

### Scenario 2: Toggling back to light mode
*   **Given** the user is viewing the page with "dark" theme enabled
*   **When** they click the theme toggle button in the Header
*   **Then** the theme should switch back to "light"
*   **And** the `dark` class should be removed from the document body or root HTML element
*   **And** the toggle button icon should change back to a Sun icon.

## 4. Technical Constraints & Design Systems
*   **Do's**:
    - [x] Use icons from the existing `lucide-react` library: `Sun` and `Moon`.
    - [x] Align the toggle button to the far right of the navigation links in the Header component.
    - [x] Apply a subtle micro-animation transition when switching icons (e.g., rotation or fade).
*   **Don'ts**:
    - [x] Do not write direct localStorage logic in the Header. Use the existing `toggleTheme` method from `ThemeContext` which handles persistence automatically.

## 5. Verification & Testing Instructions
*   **Automated Verification**:
    - Run unit tests: `npm run test src/components/__tests__/Header.test.jsx`
    - Verify builds: `npm run build`
*   **Manual Verification Steps**:
    1. Start the app locally: `npm run dev`.
    2. Click the Sun icon in the top-right header.
    3. Verify that the background transitions to dark and the text changes to white.
    4. Confirm that the icon switches to a Moon icon.
    5. Refresh the page and ensure the dark theme state is maintained.

## 6. References & Attachments
*   **Design Link**: Figma prototype at `https://figma.com/file/mock-project-design#Header-Darkmode`
*   **Related Issues**: Epic FEAT-800 (Accessibility and Personalization features)
