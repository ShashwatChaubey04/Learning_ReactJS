# Styled Components

What it is: A way to write CSS inside your JavaScript code in React.
Why use it: Because it keeps styles tied to the component, so no messy global CSS.

Example:-

import styled from 'styled-components';
const Button = styled.button`
  background-color: blue;
  color: white;
  padding: 10px;
`;
function App() {
  return <Button>Click Me</Button>;
}

Easy way to remember: “CSS lives inside the component, and you can use JavaScript inside it.”



# Sass

What it is: A CSS preprocessor. Think of it as “CSS with superpowers.”
Superpowers:-
Variables: Store colors, sizes, etc.
Nesting: Write CSS inside CSS instead of repeating selectors.
Mixins & functions: Reuse styles easily.

# SCSS

What it is: A syntax of Sass that looks almost like normal CSS.
Difference: Sass has two styles:
Indented syntax (.sass) – no curly braces {} or semicolons ;
SCSS syntax (.scss) – like CSS with {} and ; (most people use this)

$primary-color: blue;
.button {
  background-color: $primary-color;
  padding: 10px;

  &:hover {
    background-color: darkblue;
  }
}