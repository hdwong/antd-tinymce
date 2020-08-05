# Antd-TinyMCE

TinyMCE Rich-Text-Editor for Ant.Design

## Including in node

    npm install antd-tinymce

Then it can be imported in your script like so:

```js
import AntdTinymce from 'antd-tinymce';

// Set APIKey
AntdTinymce.config('xxxxxx');

// Change default options
AntdTinymce.setDefaultPlugins('');
AntdTinymce.setDefaultMenubar('');
AntdTinymce.setDefaultToolbar('');
AntdTinymce.setDefaultOptions({});

// @see https://www.tiny.cloud/docs/configure/integration-and-setup/ for more information about configuration
```

## Usage
```jsx
import React from 'react';
import { Form } from 'antd';
import AntdTinymce from 'antd-tinymce';

class Test extends React.Component {
  render() {
    return (
      <Form initialValues={{text:'<h1>Hello World</h1>'}}>
        <Form.Item name="text">
          <AntdTinymce
              options={{ height: 500 }}
              plugins=''
              menubar=''
              toolbar='' />
        </Form.Item>
      </Form>
    );
  }
}
```
