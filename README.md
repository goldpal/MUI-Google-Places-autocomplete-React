# MUI Google Places Autocomplete

React component for easily use Google Places Autocomplete, which uses the MUI [React Autocomplete component](https://mui.com/material-ui/react-autocomplete).

> **Warning**    
> This is currently pre-production - don't expect it to work right now.

<p align="center"><img width="413" alt="a screenshot showing the component in action." src="https://user-images.githubusercontent.com/7024578/209857174-317d4f60-e187-467e-bf20-3bb0bf6c4678.png"></p>


## Getting started

Install the latest version:

```sh
npm install --save mui-google-places-autocomplete
  or
yarn add mui-google-places-autocomplete
```

Use the component:

```jsx
import React from "react";
import GooglePlacesAutocomplete from "@dylmye/mui-google-places-autocomplete";

const Component = () => (
  <div>
    <GooglePlacesAutocomplete apiKey="****" />
  </div>
);

export default Component;
```

Or with [Formik](https://formik.org/):

```jsx
import React from "react";
import { Formik, Form, Field } from "formik";
import { GooglePlacesAutocompleteField } from "@dylmye/mui-google-places-autocomplete";

const MyForm = () => (
  <Formik onSubmit={console.log}>
    <Form>
      <Field
        name="location"
        component={GooglePlacesAutocompleteField}
        apiKey="****"
      />
    </Form>
  </Formik>
);

export default MyForm;
```