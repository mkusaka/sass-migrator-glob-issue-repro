# sass-migrator-glob-issue-repro

## step
1. clone this repository
2. yarn install
3. run `yarn reproduce`

### actual

```
❯ yarn reproduce
yarn run v1.22.19
$ sass-migrator division "src/#styles/style.scss"
Error: Could not find Sass file at 'src/#styles/style.scss'.
Migration failed!
error Command failed with exit code 1.
info Visit https://yarnpkg.com/en/docs/cli/run for documentation about this command.
```

### expected
Works with no error as `yarn works` output

```
❯ yarn works    
yarn run v1.22.19
$ sass-migrator division "src/styles/style.scss"
Nothing to migrate!
```
