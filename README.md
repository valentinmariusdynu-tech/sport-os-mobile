# sport-os-mobile

[![CI](https://github.com/valentinmariusdynu-tech/sport-os-mobile/actions/workflows/ci.yml/badge.svg)](https://github.com/valentinmariusdynu-tech/sport-os-mobile/actions/workflows/ci.yml)

React Native + Web hybrid app for the Sport-OS platform — athlete dashboard, live event tracking, and SFR device pairing.

## Stack
Expo SDK · React Native · TypeScript · Zustand · Expo Router · React Query

## Architecture
```
src/
├── app/          — Expo Router file-based routes
├── components/   — shared UI components
├── hooks/        — custom React hooks
├── stores/       — Zustand state stores
├── services/     — API client (sport-os-backend)
└── lib/          — utilities, types, constants
assets/           — fonts, images, icons
```

## Quick Start
```bash
npm install
npx expo start
# iOS: press i  |  Android: press a  |  Web: press w
```

## Dev Commands
```bash
npx tsc --noEmit                    # type check
npm test                            # jest
npm run lint                        # eslint
npx expo export --platform web     # production web build
```

## Related Repos
| Repo | Role |
|---|---|
| [sport-os-backend](https://github.com/valentinmariusdynu-tech/sport-os-backend) | Backend API |
| [sport-os-ai](https://github.com/valentinmariusdynu-tech/sport-os-ai) | AI features |
| [sport-os-infra](https://github.com/valentinmariusdynu-tech/sport-os-infra) | Infrastructure |
| [sport-os-docs](https://github.com/valentinmariusdynu-tech/sport-os-docs) | Documentation |
| [sfr-firmware](https://github.com/valentinmariusdynu-tech/sfr-firmware) | SFR device firmware |
