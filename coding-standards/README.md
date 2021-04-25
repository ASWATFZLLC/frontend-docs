### Coding standards
#### Note
- Restrain from using Subscription unless it makes sense (use subscription.toPromise())
#### Dependencies
- Avoid `~` and `^` in dependencies. Instead target specific version (reduce upgrade "noise")
- If you need to target a previous version, please explain the reason with a note
#### Styles
DO:
1. Use 2 spaces per indentation
2. Use Single Quote only `'`
3. ~~Surround loop and conditional bodies with curly braces. Even for single line statement.~~
4. ~~Commas `,`, colons `:` and semi-colons `;` are followed by a single space~~
5. End of statement must be followed by semi-colons `;` even if not required

DO NOT:
1. Do not use `var` to declare variable. Instead use `const` or `let`
2. ~~Do not use `<type>myVar` for casting. Instead use `as` keyword~~
3. Do not declare multiple variables with a single variable statement (`let x = 1, y = 2` is forbidden)
4. Avoid anonymous functions. Instead use arrow functions. (Only few exceptions)
#### Files & Declaration
DO:
1. 1 file per logical component

DO NOT:
1. Do not export type/functions/interface/class unless you need to share it across multiple components
#### Names
DO:
1. Use PascalCase for type names
2. Use PascalCase for enum values
3. Use camelCase for function names
4. Use camelCase for property name and local variables
5. Use whole words when possible. ~~One letter variable names are only allowed in arrow functions~~

DO NOT:
1. Do not use `I` as a prefix for interface names
#### Types
DO:
1. Variable must all be typed. Type may be omitted if the variable is assigned in the same statement
2. Function must all have a return type (even `void`)

DO NOT:
1. Do not use anonymous types. Instead use `Interface`
2. Do not use `'x'|'y'`' as type. Instead use `Enum`
3. Avoid using type `any`