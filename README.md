1.fnm use 19
    powershell:
        fnm env --use-on-cd | Out-String | Invoke-Expression
    cmd:
        FOR /f "tokens=*" %i IN ('fnm env --use-on-cd') DO CALL %i
2.
    macos
        cp $(command -v node) hello
    windows:
        cmd:
            x=where node 
            copy x hello.js
        powershell:
             Copy-Item (Get-Command node).Source portable
3.
    macos
        codesing --remove-signature hello
4.
    hello.js
        console.log(`Hello, ${process.argv[2]}!`)
5.
     npx postject hello NODE_JS_CODE hello.js \ --sentinel-fuse NODE_JS_FUSE_fce680ab2cc467b6e072b8b5df1996b2
6. 
    macos
        codesing --sing - hello
7.  delete hello.js 
8.  rename hello -> hello.js
9.  ./hello Twitch