# jsQuizizz
[![NPM](https://img.shields.io/npm/v/jsquizizz?color=darkcyan&logo=npm&style=for-the-badge&label=Version)](https://nodei.co/npm/jsquizizz/)
---
## Overview
jsQuizizz is a NodeJS Wrapper for the Quizizz API.

## Installing
> The package is not uploaded to NPM yet
This package can be installed using NodeJS's package manager, `npm`.
```bash
npm install jsquizizz
```

## Importing
> To use the new esm syntax, set your `type` to `module` in your `package.json`. [Click me](https://nodejs.org/api/packages.html#packages_package_json_and_file_extensions) for more information
- You can import the entire package into a single variable (***esm***)
    ```js
    import * as Quizizz from 'jsquizziz'
    ```

- You can import certain parts of the package into different variables (***esm***)
    ```js
    import {MemeSet, Quiz, Tag, User, Game} from 'jsquizziz'
    ```
- You can also import this package into non-esm modules (***commonjs***)
    ```js
    var Quizizz = await import("jsquizizz")
    ```

## Documentation
- ### MemeSet
    Quizizz shows the players memes after every question answered. These memes are stored in MemeSets, and the `MemeSet` class allows us to get these MemeSets

    - **Importing**
        ```js
        import {MemeSet} from 'jsquizizz'
        ```
    - **Functions**
# jsQuizizz
[![NPM](https://img.shields.io/npm/v/jsquizizz?color=darkcyan&logo=npm&style=for-the-badge&label=Version)](https://nodei.co/npm/jsquizizz/)
---
## Overview
jsQuizizz is a NodeJS Wrapper for the Quizizz API.

## Installing
> The package is not uploaded to NPM yet
This package can be installed using NodeJS's package manager, `npm`.
```bash
npm install jsquizizz
```

## Importing
> To use the new esm syntax, set your `type` to `module` in your `package.json`. [Click me](https://nodejs.org/api/packages.html#packages_package_json_and_file_extensions) for more information
- You can import the entire package into a single variable (***esm***)
    ```js
    import * as Quizizz from 'jsquizziz'
    ```

- You can import certain parts of the package into different variables (***esm***)
    ```js
    import {MemeSet, Quiz, Tag, User, Game} from 'jsquizziz'
    ```
- You can also import this package into non-esm modules (***commonjs***)
    ```js
    var Quizizz = await import("jsquizizz")
    ```

## Documentation
- ### MemeSet
    Quizizz shows the players memes after every question answered. These memes are stored in MemeSets, and the `MemeSet` class allows us to get these MemeSets

    - **Importing**
        ```js
        import {MemeSet} from 'jsquizizz'
        ```
    - **Functions**
        | **Type**  | **Method**        | **Parameters** | **Returns**          | **Description**                          | **Example**                                                    |
        |-----------|-------------------|----------------|----------------------|------------------------------------------|----------------------------------------------------------------|
        | `static`  | `getByID`         |                | `Promise<MemeSet>`   | Gets a MemeSet via it's ID               | ```js await MemeSet.getByID("abcdef", false) ```               |
        | `static`  | `getFromUser`     |                | `Promise<MemeSet[]>` | Gets a list of MemeSets from a user's ID | ```js await MemeSet.getFromuser("abcdef") ```                  |
        | `static`  | `getFeatured`     | None           | `Promise<MemeSet[]>` | Gets the currently featured MemeSets     | ```js await MemeSet.getFeatured() ```                          |
        | `dynamic` | `getMemes`        |                | `Promise<Meme[]>`    | Gets the memes from the MemeSet          | ```js await myMemeSet.getMemes(true) ```                       |
        | `dynamic` | `Meme.getCreator` | None           | `Promise<User>`      | Gets the meme's creator.                 | ```js await (await myMemeSet.getMemes(false))[0].getCreator(); |
- ### Quiz
- ### Tag
- ### User
- ### Game
- ### Quiz
- ### Tag
- ### User
- ### Game

<table class="tg">
<thead>
  <tr>
    <th>Type</th>
    <th>Method</th>
    <th>Parameters</th>
    <th>Returns</th>
    <th>Description</th>
    <th>Example</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>
    
`static`</td>
    <td>
`getByID`</td>
    <td></td>
    <td>

`Promise<MemeSet>`
    </td>
    <td>Gets a MemeSet via it's ID</td>
    <td>
```js
await MemeSet.getByID("abcdef", false)
```
 </td>
  </tr>
  <tr>
<td>

`static`
</td>
    <td>

`getFromUser`</td>
    <td></td>
    <td>`Promise<MemeSet[]>`</td>
    <td>Gets a list of MemeSets from a user's ID</td>
    <td>
```js
await MemeSet.getFromuser("abcdef")
```
</td>
  </tr>
  <tr>
    <td>
    
`static`</td>
    <td>
    
`getFeatured`</td>
    <td>None</td>
    <td>`Promise<MemeSet[]>`</td>
    <td>Gets the currently featured MemeSets</td>
    <td>```js<br>await MemeSet.getFeatured()<br>```</td>
  </tr>
  <tr>
    <td>`dynamic`</span></td>
    <td>`getMemes`</span></td>
    <td class="tg-0pky"></td>
    <td>`Promise&lt;Meme[]&gt;`</span></td>
    <td class="tg-0pky">Gets the memes from the MemeSet</td>
    <td class="tg-0pky">```js<br>await myMemeSet.getMemes(true)<br>```</td>
  </tr>
  <tr>
    <td>`dynamic`</span></td>
    <td>`Meme.getCreator`</span></td>
    <td class="tg-0pky">None</td>
    <td>`Promise&lt;User&gt;`</span></td>
    <td class="tg-0pky">Gets the meme's creator.</td>
    <td class="tg-0pky">```js<br><br>await (await myMemeSet.getMemes(false))[0].getCreator();<br>```</td>
  </tr>
</tbody>
</table>#   j s Q u i z i z z  
 