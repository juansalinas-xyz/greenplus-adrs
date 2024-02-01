# Framework CSS

- Status: accepted <!-- optional -->
- Deciders: - <!-- optional -->
- Date: 31/01/24 <!-- optional. To customize the ordering without relying on Git creation dates and filenames -->

## Context and Problem Statement

We need to create a small application in a short time.

## Decision Drivers <!-- optional -->

- Easy implementation
- Fast learning
- Should be easy to integrate MUI to the project with this framework.

## Considered Options

- [Tailwindcss](https://tailwindcss.com/)
- [SCSS](https://sass-lang.com/)
- [CSS Modules](https://nextjs.org/docs/app/building-your-application/styling/css-modules/)
- [Material-UI](https://mui.com/)

## Decision Outcome

Chosen option: "Material-UI" and "Tailwindcss", because it is the option that will give us more speed and dynamism, to achieve not only good results, but also agility.

### Positive Consequences <!-- optional -->

- Easy implementation
- Creation speed
- Easy learning
- Good design

### Negative Consequences <!-- optional -->

- Generic aesthetics

## Pros and Cons of the Options <!-- optional -->

### Tailwindcss

- Good, summarized syntax
- Good, it is not necessary to change files to make changes.
- Good, Easy to use and learn.
- Good, you won't have to use your time to name classes.
- Good, Tailwind classes are designed to be independent and are not tied to the HTML structure. This encourages loose coupling between design and application logic, facilitating maintenance and scalability.
- Good, Tailwind easily integrates with JavaScript and front-end frameworks.
- Bad, it can get very verbose.
- Bad, it can be messy, and therefore confusing for those who read it.
- Bad, if you end up saving portions of code in variables, you would be losing the convenience of not thinking about class names.
- Bad, When applying classes directly to the HTML, the HTML file can become larger and contain a considerable number of classes. This can affect the readability of the HTML, especially in large projects.
- Bad, initial setup may take time to adjust to project preferences.
- Bad, For projects with very specific and unique design requirements, Tailwind's utilitarian approach might not be the best option.
- Bad, if not applied consistently, heavy use of utility classes could result in inconsistencies in styling between different parts of the application, especially in large teams where multiple developers work on the same project.

### SCSS

- Good, syntax identical to CSS but improved.
- Good, you can organize the code better.
- Good, the nesting of selectors in SCSS helps to organize the code more hierarchically, making the CSS structure more intuitive and easier to understand.
- Good, has code blocks that can be reused.
- Good, includes mathematical operators and functions that allow calculations and value manipulations to be performed directly in the code, which can simplify design.
- Good, You can nest media queries rules directly inside selectors, which helps keep associated rules together.
- Bad, the learning curve can be challenging for beginners.
- Bad, although nesting selectors can improve readability, abuse of this feature can lead to the generation of overly specific and difficult to maintain CSS code.
- Bad, in small or simple projects, the introduction of a preprocessor such as SCSS may be considered unnecessary and add additional complexity to the development process.
- Bad, if not configured properly, it can cause maintenance problems, especially in teams where not all members are familiar with Sass.

### CSS Modules

- Good, one of the main advantages is that it encapsulates styles within modules, avoiding name conflicts and style collisions between different parts of the application. Each module has its own scope, making development and maintenance easier.
- Good, by reducing interference between styles of different parts of the application, facilitates teamwork.
- Good, is especially beneficial in large and scalable projects. As the application grows, encapsulation and scoping help avoid common problems associated with maintaining large style code bases.
- Bad, in small or simple projects, the introduction of CSS modules may be considered unnecessary and add additional complexity to the development process.
- Bad, If the code is divided too much into many small modules, it could lead to excessive granularity and increase maintenance complexity.
- Bad, in large projects, generating unique identifiers for each class can result in increased compile time.
- Bad, some third-party tools and libraries may not be supported natively

### Material-UI

- Good, ready-to-use components, Material UI provides a wide range of ready-to-use UI components, this can significantly speed up development.
- Good, consistent themes and styles, Material UI components follow the Material Design design guide. This provides visual consistency throughout the application.
- Good, Responsive, Material UI components are designed to be responsive and work well on different screen sizes.
- Good, customizable, components can be easily customized with the theme system to match your brand.
- Good, large community, Material UI has a large community so it's easy to get help and support.
- Bad, learning curve, it may take some time to get familiar with all the available components and how to customize them.
- Bad, package size, Material UI is quite large and can significantly increase the package size of your app.
- Bad, frequent releases, Material UI releases new versions frequently, so you may have to update often.
- Bad, not always native, components don't always behave exactly like native controls, which may confuse some users.
