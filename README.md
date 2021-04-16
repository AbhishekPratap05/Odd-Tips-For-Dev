## Useful tips here 👇 to make developers happy 😄

<details>
<summary><b style="font-size:24px">To search and delete node_modules from older projects.🚮</b></summary>

#### we all suddenly face problem with device space  getting full, main culprit for us developers is dependencies (node_modules), it can be more than 300MB+ 😲 for react and more if you add more dependencies later on, which we all do 🤦‍♂️.
#### There is a awesome tool to kill them, i mean not really kill but delete.
#### **[npkill](https://npkill.js.org/)** is just awesome easy to use cli tool.

- #### You can install globally by running 
```
$ npm i -g npkill
```
> #### Make sure you have node installed 

- #### You can also use it without installing it by running
```
$ npx npkill
```
<p align="center">
  <img src="https://npkill.js.org/img/start%20search.gif" width="48%" title="start search" alt="npkill searching">
  <img src="https://npkill.js.org/img/deleting.gif" width="48%" title="deleting" alt="npkill deleting">
</p>

<details>
<summary><span style="font-size:18px;color:#FF5733">Some Useful commands</span></summary>
<p>
<ui>
<li>Search node_modules directories in your projects directory</li>
<code>$ npkill -d ~/projects</code></br></br>
<li>Displays the magenta color cursor... because I like magenta!</li>
<code>$ npkill --color magenta</code></br></br>
<li>List directories called "dist" and and show errors if any occur:</li>
<code>$ npkill --target dist -e</code></br></br>
<li>List vendor directories in your projects directory, sort by size, and show that in gb:</li>
<code>$ npkill -d '~/more projects' -gb --sort size --target vendor</code>
</ul>
</p>
</details>
</details>

</br>

<details>
<summary><b style="font-size:24px">To fix long import relative paths for project.🖇</b></summary>

#### We all have file path looked like this `../../../../../` so on. At some point it feels like we are importing something out of project, if you have not been there than you are lucky or have great folder structure and if you have one contact me 😉.
#### There is an easy solution for VS Code users, sorry for the 1% people who are not using VS Code. 😆
#### Steps to be followed :
- create `jsconfg.json` file in your project root directory.
- Inside file map paths in your project using keyword.
  ```
  {
    "compilerOptions": {
      "baseUrl": "./",
      "paths": {
        @components/*": ["components/*"]
        @lib/*": ["lib/*"]
        @styles/*": ["styles/*"]
      }
    }
  }
  ```
  #### 🎉 Done 🎊 yes its that simple, and for to use this in your file just replace the `../../../../../SomeComponent` with `@components/SomeComponent`.
</details>

