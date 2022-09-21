# Story Component :rocket: :100: :rocket:
A Component for rendering a Story of Components with different variants or args

#### Just Copy the `Story Component` folder in your app `components` folder.

### Usage Example

A Story of a Button Component

```js
import Stories from 'components/Story Component'
import Button from 'components/button'

// args
const primary = { arg: 'Primary', label: 'Primary', variant: 'secondary' }
const secondary = { arg: 'Secondary', label: 'Secondary', variant: 'secondary' }
const rounded = { arg: 'Rounded', label: 'Rounded', variant: 'rounded' }
const error = { arg: 'Error', label: 'Error', variant: 'error' }

const ButtonStory = () => (
  <Stories
    argList={[primary, secondary, rounded, error]}
    template={args => <Button {...args} />}
  />
)

export default ButtonStory
```

### Story Component Props

```js
  argList: PropTypes.array.isRequired,
  template: PropTypes.func.isRequired,
  customClass: PropTypes.string,
```
