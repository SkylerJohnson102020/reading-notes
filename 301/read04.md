# Forms in React

https://reactjs.org/docs/forms.html

- Forms are different from other HTML elements since they already keep some form of internal state. It has a default of going to a new page in a browser. This simply works this way in React. Examples would be your input, textarea, and select tags.

- Controlled Components - While form elements usually maintain their own state, React keeps mutable state in components in their state prop and update state with setState. A controlled component is the combination of these two. So, React has full control of both the rendering of the form and the user input.

- The value of an input is always guided by state in controlled components.

- form element need:

        this.state = {value: ''}; //in constructor

        handleEventChange(event) { //handler (added after constructor in example)
            this.setState({value: event.target.value});
        }

        <form onSubmit={this.handleSubmit}> // added to the render method
            <label>
                Name:
                <input type="text" value={this.state.value} onChange={this.handleEventChange} />
             </label>


- textarea tag will take a "value" att instead of a "type" att in the label of the form element.

- select tag - Creates drop down list. (You will need to use the option tag to list your items.) One item has a selected att showing that is initially selected.

- file input tag - user can choose one or multiple files. This is managed by JS through the File API. This is an uncontrolled component since the value is read-only. **See example in article for more in-depth explantion.**

ES6 computed property name:

        this.setState({
            [name]: value
        });

- Controlled input null value - specify this in the value prop. Setting this will prevent a user from changing the input unless you want them to. You can set a timeout to where it will say something like "hello" then become editable after a short period of time, maybe a few seconds.

- Checkout Formik - helps handle a lot of "under the hood" activity with the forms.

[code301 Reading Notes](/301/code301Table.md)