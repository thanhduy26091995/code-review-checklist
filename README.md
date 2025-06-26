# 📱 Mobile Code Review Checklist

## 1. Code Quality
- [ ] Code follows platform/language-specific style guides (e.g., SwiftLint, Ktlint)
- [ ] Code is clean, readable, and consistently formatted
- [ ] Uses descriptive names for variables, methods, and classes
- [ ] Avoids deep nesting and large functions
- [ ] No commented-out or unused code left behind

## 2. Architecture & Design
- [ ] Follows established architecture (MVVM, MVI, Clean Architecture, etc.)
- [ ] Code is modular and adheres to separation of concerns
- [ ] Logic is encapsulated in ViewModels/UseCases, not UI controllers
- [ ] Dependency injection is used where appropriate

## 3. Functionality
- [ ] Feature works as intended and matches requirements
- [ ] Validates user inputs correctly
- [ ] Handles offline/poor network conditions gracefully
- [ ] Appropriate error handling and user feedback is provided

## 4. UI/UX
- [ ] Layout works on various screen sizes and orientations
- [ ] Animations and transitions are smooth and appropriate
- [ ] Follows platform design guidelines (Material Design / Human Interface)
- [ ] Accessibility (a11y) features like TalkBack/VoiceOver are supported
- [ ] Font sizes and touch targets meet accessibility standards

## 5. Performance
- [ ] Avoids unnecessary recompositions or view redraws
- [ ] Images are optimized and properly cached
- [ ] Network and database operations are performed asynchronously
- [ ] Lazy loading and pagination are used where applicable
- [ ] Memory usage is monitored (no leaks, OOM risk, etc.)

## 6. Security
- [ ] No hardcoded secrets, keys, or credentials in the code
- [ ] Secure storage used for sensitive data (e.g., Keychain, EncryptedSharedPreferences)
- [ ] Permissions are requested only when needed
- [ ] Input is validated and sanitized to avoid injection or crashes
- [ ] Code is obfuscated/minified if required for release builds

## 7. Testing
- [ ] Unit tests cover core logic
- [ ] UI/E2E tests exist for main flows (Espresso, XCTest, Detox, etc.)
- [ ] No flaky or slow tests
- [ ] Tests are run in CI and pass consistently
- [ ] Mocks/Fakes used for dependencies in unit tests

## 8. Build & Configuration
- [ ] Build variants (debug/release) are configured correctly
- [ ] API endpoints, keys, and flags are environment-specific
- [ ] Proguard/R8 (Android) or Bitcode settings (iOS) are correct
- [ ] Gradle/Xcode build scripts do not include temporary hacks
- [ ] Third-party dependencies are up-to-date and approved

## 9. Analytics & Monitoring
- [ ] Events and screen tracking are added where needed
- [ ] Crash reporting is integrated and tested (e.g., Firebase Crashlytics, Sentry)
- [ ] Logs do not expose sensitive or verbose data
- [ ] Logging levels are appropriate for debug vs. release builds

## 10. Version Control
- [ ] Small, meaningful commits
- [ ] No generated files (e.g., `.DS_Store`, `*.iml`, `build/`) are committed
- [ ] `.gitignore` is respected
- [ ] PR description includes context, screenshots, and test steps
- [ ] Feature branch is up to date with base branch

---

## 🛠 Optional CI/CD Automation
- [ ] Linting (SwiftLint, Ktlint, Dart Analyzer)
- [ ] Static code analysis (e.g., SonarQube, Detekt)
- [ ] Test runs for unit/UI tests
- [ ] App build + artifact upload (e.g., Firebase App Distribution, TestFlight)
- [ ] Security scan (e.g., MobSF, Snyk for mobile)

