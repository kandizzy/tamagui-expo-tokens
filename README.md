# Example with error: 

```
(base) user@computer tamagui-expo-tokens % npm start

> expo-router@1.0.0 start
> expo start

Starting project at ~/tamagui-repro/tamagui-expo-tokens
Starting Metro Bundler

    ➡ [tamagui] built config and components (487ms):

        Config     ./.tamagui/tamagui.config.cjs
        Components ./.tamagui/tamagui-components.config.cjs
        
  tamagui: skipping ~/tamagui-repro/tamagui-expo-tokens/.tamagui/tamagui.config.cjs tamagui.dev/docs/intro/errors#warning-001
~/tamagui-repro/tamagui-expo-tokens/node_modules/@tamagui/web/dist/cjs/createVariable.js:71
    throw new Error(`createCSSVariable expected string, got: ${nameProp}`);
          ^

Error: createCSSVariable expected string, got: undefined
    at createCSSVariable (~/tamagui-repro/tamagui-expo-tokens/node_modules/@tamagui/web/src/createVariable.ts:98:13)
    at variableToCSS (~/tamagui-repro/tamagui-expo-tokens/node_modules/@tamagui/web/src/helpers/registerCSSVariable.ts:10:63)
    at ~/tamagui-repro/tamagui-expo-tokens/node_modules/@tamagui/web/src/createTamagui.ts:129:29
    at createTamagui (~/tamagui-repro/tamagui-expo-tokens/node_modules/@tamagui/web/src/createTamagui.ts:194:3)
    at loadTamagui (~/tamagui-repro/tamagui-expo-tokens/node_modules/@tamagui/static/src/extractor/loadTamagui.ts:61:20)
    at processTicksAndRejections (node:internal/process/task_queues:95:5)
    at Object.load [as loadTamagui] (~/tamagui-repro/tamagui-expo-tokens/node_modules/@tamagui/static/src/extractor/createExtractor.ts:137:29)
```