# Petite Vue Codebase

## What

Attached files is concatenated codebase of the framework and its dependencies.

## How

- Refer to the codebase when generating the responses
- Give special attention to how `reactive` and `components` work.

## Why

- Documentation & examples are sparse for this framework, so I need system to
  depend on.

## Instructions

- Maximise dependence on the codebase to generate solutions
- Before generating solution, cross check whether the solution is consistent to
  the dependencies

## Ask

- Reply that you are ready to assit if you understand the code & instructions.

## Coding Patterns

1. Always generate *full* code files not snippets
2. Always respect the code/dependencies already present
3. When modifying, change only the specific parts of the file required to do the
change
4. Try to adhere to the prettier.json attached
5. Tailwind 2.2.19 is used via CDN & a custom CSS file: `tw.css` is used
6. Go through tw.css to understand the meaning of the classes used
7. Study how the sample project is structured, how state is managed and how
components are split so that this pattern is used when you generate code
8. Make sure the Petite Vue components you generate are pure functions with no
dependencies except the utility classes of Tailwind 2.2.19 (CDN version)
9. If a markup is provided to convert to PV, try to extract props & build a pure
function PV component

## Component Generation

If asked to generate a PV component follow these instructions closely:

### Hard Constraints

1. ONLY generate the PV component as PURE JS code
2. Don't use `reactive` in components
3. Use tailwind classes (v2.2.19)
4. Avoid explanations
5. Extract props into good variable names
6. Provide default values for props
7. Extract hanlders, provide default values that logs the arguments
8. Avoid PV import and createApp function
9. Use `const Component = () =>` than `function Component` style
10. Build beautiful components
11. Caution: Store the variables & functions in the return object of the
component thats needed in the template.
12. Note: If component is requested for CodePen, name the component Example
13. Never hard code data inside component
14. If default values are going to be long, define them in separate variable
outside the component
