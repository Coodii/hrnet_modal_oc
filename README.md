# hrnet_modal_oc

hrnet_modal_oc is a simple and reusable modal component for React

## Installation

The package can be installed via [npm](https://www.npmjs.com)

```bash
npm i hrnet_modal_oc
```

Or via [Yarn](https://yarnpkg.com/)

```bash
yarn add hrnet_modal_oc
```

## Configuration

#### 1. import

When you need the modal component, you have to import the component in your file

```js
import { Modal } from 'hrnet_modal_oc'
```

#### 2. Required props

To run this modal, 3 props are required

```js
title, //String
content, //String
setModal, // Boolean
```

## Example

Basic example

```js
import React, { useState } from 'react'
import { Modal } from 'hrnet_modal_oc'

const Example = () => {
  const [modal, setModal] = useState(false);
  return (
    <div>
      <button onClick={() => setModal(true)}>Open modal</button>
      <Modal setModal={setModal} title='Modal' content='Lorem ipsum dolor sit amet, consectetur adipiscing elit...'/>
    </div>
  )
}
```