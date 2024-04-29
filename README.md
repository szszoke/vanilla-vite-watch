# Issue

`No CSS for` error is thrown when vite build is started in watch mode and files are changed.

## Steps to reproduce

1. `npm install`
2. `npx vite build --watch`
3. Make a change in `test-style.css.ts` and save the file

## Expected result

`style.css` is generated.

## Actual result

`No CSS for` errors thrown and no `style.css` is generated.

# Remarks

A patch in the `patches` directory is available that resolves the issue. It can be applied by running `npx patch-package`.