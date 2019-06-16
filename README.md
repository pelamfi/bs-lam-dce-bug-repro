# bs-lam-dce-bug-repro

Minimal reproduction of a possible compiler bug I encountered
when using the bs-platform version 5.0.4.

## Installing NPX for using `bs-platform` from `node_modules`

```sh
npm install -g npx
```

## Reproducing the bug

Running:

```sh
npm run start
```

Produces the following output on my Mac:

```

> bs-lam-dce-bug-repro@0.1.0 start ###/bs-lam-dce-bug-repro
> npx bsb -make-world -w

>>>> Start compiling 
[2/2] Building BsLamDceBugRepro.cmi
[1/1] Building src/Problem-BsLamDceBugRepro.cmj
Fatal error: exception Failure("File \"lam_dce.ml\", line 46, characters 40-47intValue/1014 not found")
```
