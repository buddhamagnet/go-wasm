### GOLANG WASM FTW

* Compile main function with ```GOARCH=wasm GOOS=js go build -o lib.wasm main.go```
* This will drop a binary called ```lib.wasm``` into the current directory.
* Copy the required file ```cp "$(go env GOROOT)/misc/wasm/wasm_exec.js" .```
* Check the index page, which includes the above file and polyfills WASM streaming if not available.
* Runs the function in main when you click the button!