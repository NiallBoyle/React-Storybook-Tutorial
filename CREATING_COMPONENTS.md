
# React Native Storybook Tutorial

In this tutorial i'll be showing you how to create a react component from a figma design.




## Figma Link

https://www.figma.com/file/81y668umjUp8CZW3Kx9fy1/React-Native-Storybook-Tutorial?type=design&node-id=0%3A1&mode=design&t=wGecNyoW8GD77H85-1
## Creating Components

**`1`** Click the Figma link and sign up for Figma.

**`2`** Click the button on the top right corner to enable developer mode "</>".

**`3`** Click on the component you would like to create.

**`4`** On the right panel click "Plugins".

**`5`** Search for the plugin "Vigma RN".

**`6`** Copy the code.

**`7`** Create a new file *COMPONENT_NAME.js*.

**`8`** Paste the code you copied into the new file you created.

**`9`** Change **`export default function`** to **`export const COMPONENT_NAME = () => {}`** in *COMPONENT_NAME.js*

**`10`** Import any missing packages **`yarn add PackageName`**

**`11`** Create a story file for that component *COMPONENT_NAME.stories.js*.

**`12`** Copy the code from the template story file into your story file, import and pass in the component you created.

**`13`** Create variants and pass in arguments you may have created for this component.

**`14`** Run **`yarn storybook:ios`** / **`yarn storybook:android`** in the console and wait for the simulator to open.

**`15`** Click "**SIDEBAR**" at the bottom left and click on your newly created component.
## Creating Props

**`1`** Within your component inside the round brackets (**`export const COMPONENT_NAME = () => {}`**) you can create different props that you can pass through your component.

**`export const COMPONENT_NAME = (PropName1, PropName2) => {}`**

**`2`** You can then pass in where you'd like the prop to be populated wthin your component by using the curly brackets.

**`{PropName1}`**

**`3`** You can then populate these props within your stories by passing them in through the arguments within your story file.

**`export const Default = {args: {PropName1: VALUE, PropName2: "VALUE"}}`**

**`4`** When storybook is running you can change the value of the props by clicking the icon on the bottom right that will display all the controls.


## Creating Variants

Each story file within Storybook has a default story but you can create multiple different stories with different arguments.

**`1`** Under the default story you can create another story with different arguments

**`export const NewStory = {args: {PropName1: "VALUE", PropName2: Value}}`**