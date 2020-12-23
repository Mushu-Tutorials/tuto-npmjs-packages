# Host packages on npmjs.org

- Link to the official tutorial : [here](https://docs.npmjs.com/creating-and-publishing-scoped-public-packages)
- Link to my first NPM repository : [@mushuledragon/tuto-npmjs-packages](https://npmjs.com/package/@mushuledragon/tuto-npmjs-packages)

Here are steps to host package for a user (for an organization please refer to the link documentation ahead):

```shell
npm -v

cd tuto-npmjs-packages

# Create .gitignore file
echo '# NPM packages
node_modules/
' > .gitignore

npm login
npm whoami
# npm init --scope=@my-username
npm init --scope=@mushuledragon

# Test the package before publishing
npm install my-package

# Publish to npmjs.org
## Move to the root directory package
cd /path/to/package
npm publish --access public
```
