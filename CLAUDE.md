# sport-os-mobile — Stack Conventions

## Stack
- React Native + Expo SDK 51+ (iOS & Android)
- Web: Expo Router with react-native-web (shared codebase)
- TypeScript 5 strict mode
- State: Zustand
- Navigation: Expo Router (file-based)

## Code Conventions
- Prettier for formatting; ESLint (eslint-config-expo)
- Components: PascalCase; hooks: useCamelCase
- No default exports except app/ screens
- Styles via StyleSheet or NativeWind

## Testing
- Jest + React Testing Library
- E2E: Detox (mobile) / Playwright (web)

## Git
- Conventional commits; squash-merge to main
- main is always shippable to Expo EAS
