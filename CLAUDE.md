# CLAUDE.md — sport-os-mobile

## Purpose
Expo React Native app for Sport-OS: athlete dashboard, live event feed, real-time telemetry display, and SFR device Bluetooth pairing.

## Stack
- Expo SDK (latest), React Native
- TypeScript (strict)
- Expo Router (file-based routing)
- Zustand (client state), React Query (server state)
- Jest + React Native Testing Library

## Key Directories
- `src/app/` — Expo Router screens (file = route)
- `src/components/` — reusable UI components
- `src/hooks/` — custom hooks
- `src/stores/` — Zustand atoms
- `src/services/` — REST API client for sport-os-backend
- `src/lib/` — constants, types, utils

## Dev Commands
```bash
npx expo start
npx tsc --noEmit
npm test
npm run lint
```

## Conventions
- File-based routing via Expo Router — add screens by adding files to `src/app/`
- Server state in React Query; local-only state in Zustand
- Prefer `StyleSheet.create` over inline styles
- Use `expo-constants` for env values; never hardcode API URLs

## Related Repos
- [sport-os-backend](https://github.com/valentinmariusdynu-tech/sport-os-backend) — API consumed by `src/services/`
- [sfr-firmware](https://github.com/valentinmariusdynu-tech/sfr-firmware) — paired device over BLE
