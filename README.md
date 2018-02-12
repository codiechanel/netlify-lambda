## Netlify Lambda CLI

Based on Netlify-Lambda. Modified to suit personal workflow. 

Changes:

1. Removed webpack dependency. Since I create-react-app already includes webpack, it becomes redundant having 2 webpack versions co-exist in my node modules folder. 
2. Now using Babel 7. Since the new react-scripts@next uses Babel 7
3. It uses the new @babel/preset-env which allows us to target specific node versions by just adding this option: 

```javascript
{
              "presets": [
                [
                  "@babel/preset-env",
                  {
                    "targets": {
                      "node": "6.10"
                    }
                  }
                ]
              ]
            }
```

## License

[MIT](LICENSE)
