# SMS custom pre-build MFEs

## Build custom version of package

```
git checkout -b sms-v1.1.1 v1.1.1
nvm use 18
npm ci
make build
cp dist/ package
cp package.json LICENSE package/
vim package/package.json -- set correct version
tar -czf package-name-v1.1.1-sms1.tgz package
```
