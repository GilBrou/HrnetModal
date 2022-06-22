Simple modal

## Installation

To install, you can use npm or yarn:

	$ npm install modalgi
	$ yarn add modalgi

## Use

```jsx
import { useState } from "react";
import Modal from "@simple-modal-component-ab/Modal";

export const Exemple = () => {
	const [isOpened, setIsOpened] = useState(false);

	return(	
		<Modal
			isOpened={isOpened}
			onClose={() => setIsOpened(false)}
		>
			<p>Your text here</p>
		</Modal>
	)
}
```

- isOpened : boolean | Contains the state (opened or closed)
- onClose : function | Calls the function which close the modal

You can use CSS class `.modal-content` to customize style