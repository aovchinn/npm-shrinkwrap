PS C:\Users\demon\something\npm-bug> `npm config set package-lock=false`

PS C:\Users\demon\something\npm-bug> `npm config list`
```
; "builtin" config from C:\Users\demon\AppData\Roaming\npm\node_modules\npm\npmrc

prefix = "C:\\Users\\demon\\AppData\\Roaming\\npm"

; "user" config from C:\Users\demon\.npmrc

package-lock = false

; node bin location = C:\Program Files\nodejs\node.exe
; cwd = C:\Users\demon\something\npm-bug
; HOME = C:\Users\demon
; Run `npm config ls -l` to show all defaults.
PS C:\Users\demon\something\npm-bug> npm i
npm WARN old lockfile
npm WARN old lockfile The package-lock.json file was created with an old version of npm,
npm WARN old lockfile so supplemental metadata must be fetched from the registry.
npm WARN old lockfile
npm WARN old lockfile This is a one-time fix-up, please be patient...
npm WARN old lockfile

removed 2 packages, changed 1 package, and audited 5 packages in 1s

found 0 vulnerabilities
```
PS C:\Users\demon\something\npm-bug> `npm ls`
```
npm-bug@1.0.0 C:\Users\demon\something\npm-bug
`-- react@17.0.2
```
PS C:\Users\demon\something\npm-bug> `npm shrinkwrap`
```
npm notice package-lock.json has been renamed to npm-shrinkwrap.json
```