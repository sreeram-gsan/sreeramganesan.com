## Fixing the issue with sharp module in M1 Mac
<code>
xcode-select --install                  <br/>
arch -arm64 brew install gcc            <br/>
arch -arm64 brew reinstall vips         <br/>
brew info vips                          <br/>
npm install                             <br/>
</code>

## Removing lint-staged pre-commit hook.

<p>
In package-lock.json, comment the following
</p>
<code>    
// "husky": {                           <br/>
//   "hooks": {                         <br/>
//     "pre-commit": "lint-staged"      <br/>
//   }                                  <br/>
// },                                   <br/>
</code>

