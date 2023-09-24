## config\.cargo\.pre-commit\.cargo-fmt\.enable

Whether to enable cargo fmt check in pre-commit hook\.



*Type:*
boolean



*Default:*
` true `



*Example:*
` true `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/cargo\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/cargo.nix)



## config\.cargo\.pre-commit\.cargo-lock\.enable



Whether to enable cargo lock check in pre-commit hook\.



*Type:*
boolean



*Default:*
` true `



*Example:*
` true `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/cargo\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/cargo.nix)



## config\.convco\.enable



Whether to enable convco integration\.



*Type:*
boolean



*Default:*
` true `



*Example:*
` true `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/convco\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/convco.nix)



## config\.convco\.commit-msg\.enable



Whether to enable convco git commit-msg hook\.



*Type:*
boolean



*Default:*
` true `



*Example:*
` true `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/convco\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/convco.nix)



## config\.craneLib\.default



craneLib to use by default

Default value is craneLib initialized with ` config.toolchain.default `



*Type:*
attribute set



*Default:*

```
''
  crane.lib.x86_64-linux.overrideToolchain config.toolchain.default
''
```

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/crane\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/crane.nix)



## config\.craneLib\.nightly



craneLib to use when nightly toolchain is needed

Default value is craneLib initialized with ` config.toolchain.nightly `



*Type:*
attribute set



*Default:*

```
''
  crane.lib.x86_64-linux.overrideToolchain config.toolchain.nightly
''
```

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/crane\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/crane.nix)



## config\.craneLib\.stable



craneLib to use when stable toolchain is needed

Default value is craneLib initialized with ` config.toolchain.stable `



*Type:*
attribute set



*Default:*

```
''
  crane.lib.x86_64-linux.overrideToolchain config.toolchain.stable
''
```

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/crane\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/crane.nix)



## config\.env\.shellHooks



List of init hooks to execute when shell is entered



*Type:*
list of string



*Default:*

```
[
  ""
]
```

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/env\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/env.nix)



## config\.env\.shellPackages



Packages to include in all dev shells



*Type:*
list of package



*Default:*
` [ ] `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/env\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/env.nix)



## config\.git\.commit-msg\.enable



Whether to enable git pre-commit hook\.



*Type:*
boolean



*Default:*
` true `



*Example:*
` true `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/git\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/git.nix)



## config\.git\.commit-msg\.hooks



Attrset of hooks to to execute during git commit-msg hook



*Type:*
attribute set of (null or string or path)



*Default:*
` { } `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/git\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/git.nix)



## config\.git\.commit-template\.enable



Whether to enable git commit message template\.



*Type:*
boolean



*Default:*
` true `



*Example:*
` true `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/git\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/git.nix)



## config\.git\.commit-template\.body



The body of the template content



*Type:*
string or path



*Default:*

```
''
  # Explain *why* this change is being made                width limit ->|
''
```

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/git\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/git.nix)



## config\.git\.commit-template\.head



The head of the template content



*Type:*
string or path



*Default:*
` "" `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/git\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/git.nix)



## config\.git\.pre-commit\.enable



Whether to enable git pre-commit hook\.



*Type:*
boolean



*Default:*
` true `



*Example:*
` true `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/git\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/git.nix)



## config\.git\.pre-commit\.hooks



Attrset of hooks to to execute during git pre-commit hook



*Type:*
attribute set of (null or string or path)



*Default:*
` { } `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/git\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/git.nix)



## config\.git\.pre-commit\.trailing_newline



Whether to enable git pre-commit trailing newline check \.



*Type:*
boolean



*Default:*
` true `



*Example:*
` true `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/git\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/git.nix)



## config\.git\.pre-commit\.trailing_whitespace



Whether to enable git pre-commit trailing whitespace check \.



*Type:*
boolean



*Default:*
` true `



*Example:*
` true `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/git\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/git.nix)



## config\.github\.ci\.enable



Whether to enable just integration\.



*Type:*
boolean



*Default:*
` true `



*Example:*
` true `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/github\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/github.nix)



## config\.github\.ci\.workflows



Set of workflows to generate in ` .github/workflows/ `"\.



*Type:*
attribute set of (submodule)



*Default:*
` { } `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/github\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/github.nix)



## config\.github\.ci\.workflows\.\<name>\.enable



Whether this workflow file should be generated\. This
option allows specific workflow files to be disabled\.



*Type:*
boolean



*Default:*
` true `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/github\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/github.nix)



## config\.github\.ci\.workflows\.\<name>\.content



Content of the workflow



*Type:*
attribute set of anything



*Default:*
` null `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/github\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/github.nix)



## config\.just\.enable



Whether to enable just integration\.



*Type:*
boolean



*Default:*
` true `



*Example:*
` true `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/just\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/just.nix)



## config\.just\.rules



Attrset of section of justfile (possibly with multiple rules)

Notably the name is used only for config identification (e\.g\. disabling) and actual
justfile rule name must be used in the value (content of the file)\.



*Type:*
attribute set of (submodule)



*Default:*
` { } `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/just\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/just.nix)



## config\.just\.rules\.\<name>\.enable



Whether this rule should be generated\. This
option allows specific rules to be disabled\.



*Type:*
boolean



*Default:*
` true `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/just\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/just.nix)



## config\.just\.rules\.\<name>\.content



Order of this rule in relation to the others ones\.
The semantics are the same as with ` lib.mkOrder `\. Smaller values have
a greater priority\.



*Type:*
string or path



*Default:*
` 1000 `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/just\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/just.nix)



## config\.just\.rules\.\<name>\.priority



Order of this rule in relation to the others ones\.
The semantics are the same as with ` lib.mkOrder `\. Smaller values have
a greater priority\.



*Type:*
signed integer



*Default:*
` 1000 `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/just\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/just.nix)



## config\.rust\.pre-commit\.clippy\.enable



Whether to enable clippy check in pre-commit hook\.



*Type:*
boolean



*Default:*
` true `



*Example:*
` true `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/rust\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/rust.nix)



## config\.rust\.pre-commit\.leftover-dbg\.enable



Whether to enable leftover ` dbg! ` check in pre-commit hook\.



*Type:*
boolean



*Default:*
` true `



*Example:*
` true `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/rust\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/rust.nix)



## config\.semgrep\.enable



Whether to enable semgrep integration\.



*Type:*
boolean



*Default:*
` true `



*Example:*
` true `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/semgrep\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/semgrep.nix)



## config\.semgrep\.pre-commit\.enable



Whether to enable semgrep git pre-commit hook\.



*Type:*
boolean



*Default:*
` true `



*Example:*
` true `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/semgrep\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/semgrep.nix)



## config\.shareDir



Set of files that will be generated as as “Flakebox Share Dir”\.



*Type:*
attribute set of (submodule)



*Default:*
` { } `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/shareDir\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/shareDir.nix)



## config\.shareDir\.\<name>\.enable



Whether this share dir file should be generated\. This
option allows specific share dir files to be disabled\.



*Type:*
boolean



*Default:*
` true `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/shareDir\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/shareDir.nix)



## config\.shareDir\.\<name>\.mode



If set to something else than ` symlink `,
the file is copied instead of symlinked, with the given
file mode\.



*Type:*
string



*Default:*
` "symlink" `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/shareDir\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/shareDir.nix)



## config\.shareDir\.\<name>\.source



Path of the source file\.



*Type:*
path

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/shareDir\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/shareDir.nix)



## config\.shareDir\.\<name>\.target



Name of symlink (relative to share dir)\. Defaults to the attribute name\.



*Type:*
string

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/shareDir\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/shareDir.nix)



## config\.shareDir\.\<name>\.text



Text of the file\.



*Type:*
null or strings concatenated with “\\n”



*Default:*
` null `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/shareDir\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/shareDir.nix)



## config\.shareDirPackage



Derivation containing all shareDir files/symlinks



*Type:*
package

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/shareDir\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/shareDir.nix)



## config\.shellcheck\.enable



Whether to enable shellcheck integration\.



*Type:*
boolean



*Default:*
` true `



*Example:*
` true `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/shellcheck\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/shellcheck.nix)



## config\.shellcheck\.pre-commit\.enable



Whether to enable shellcheck git pre-commit hook\.



*Type:*
boolean



*Default:*
` true `



*Example:*
` true `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/shellcheck\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/shellcheck.nix)



## config\.toolchain\.channel\.default



The channel to source the default toolchain from

Defaults to the the value of the stable channel\.



*Type:*
string



*Default:*
` "stable" `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/toolchain\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/toolchain.nix)



## config\.toolchain\.channel\.nightly



The channel to source the nightly toolchain from



*Type:*
string



*Default:*
` "complete" `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/toolchain\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/toolchain.nix)



## config\.toolchain\.channel\.stable



The channel to source the stable toolchain from



*Type:*
string



*Default:*
` "stable" `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/toolchain\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/toolchain.nix)



## config\.toolchain\.components



Components to include in the default toolchains



*Type:*
list of string



*Default:*

```
[
  "rustc"
  "cargo"
  "clippy"
  "rust-analysis"
  "rust-src"
]
```

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/toolchain\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/toolchain.nix)



## config\.toolchain\.default



Default toolchain to use



*Type:*
package



*Default:*
` <derivation rust-stable-with-components-2023-08-24> `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/toolchain\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/toolchain.nix)



## config\.toolchain\.nightly



Nightly channel toolchain



*Type:*
package



*Default:*
` <derivation rust-nightly-complete-with-components-2023-09-19> `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/toolchain\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/toolchain.nix)



## config\.toolchain\.rust-analyzer



rust-analyzer package to use in the shell and lints

Separate from the toolchain as it’s common to want a custom version\.

Defaults to the standard rust-analyzer from nixpkgs input\.



*Type:*
package



*Default:*
` <derivation rust-analyzer-2023-09-11> `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/toolchain\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/toolchain.nix)



## config\.toolchain\.rustfmt



rustfmt package to use in the shell and lints

Separate from the toolchain as it’s common to want a custom (nightly) version,
for all the great yet unstable features\.

Defaults to the rustfmt from the nightly channel\.



*Type:*
package



*Default:*
` <derivation rust-nightly-complete-with-components-2023-09-19> `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/toolchain\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/toolchain.nix)



## config\.toolchain\.stable



Stable channel toolchain

Toolchain to use in situations that require stable toolchain\.



*Type:*
package



*Default:*
` <derivation rust-stable-with-components-2023-08-24> `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/toolchain\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/toolchain.nix)



## config\.typos\.enable



Whether to enable typos integration\.



*Type:*
boolean



*Default:*
` true `



*Example:*
` true `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/typos\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/typos.nix)



## config\.typos\.pre-commit\.enable



Whether to enable typos git pre-commit hook\.



*Type:*
boolean



*Default:*
` true `



*Example:*
` true `

*Declared by:*
 - [/nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/typos\.nix](file:///nix/store/sc915nnhggg1lvh8kfq6w1a9ds192xb4-source/lib/modules/typos.nix)

