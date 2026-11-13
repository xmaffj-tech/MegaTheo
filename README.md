# MegaCity
Браузерный single-player симулятор управления современными городами. Изометрическая 2D-камера, PixiJS, React и TypeScript.

## Запуск
```bash
npm install
npm run dev
```
Проверка типов: `npm run typecheck`. Production build: `npm run build`.

## Архитектура
- engine: изометрические координаты, камера, чанки и PixiJS renderer.
- simulation: дискретные расчёты населения и бюджета.
- systems: каталог и размещение зданий.
- saves: сохранения в IndexedDB.
- ui: React-панели и игровой viewport.

Мир разделён на чанки 32×32; рендеринг ограничен областью вокруг камеры.