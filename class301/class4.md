## [React Docs - Forms](https://reactjs.org/docs/forms.html)

1. What is a ‘Controlled Component’?
      * it is a component who renders a form and also controlls what happens within that form.
2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
      * the react state will hold the value of every key stroke this data won't be displayed until the submit button is pressed. havging the hamdle change function below allows the value of the state to be updated with each event. the event herebing the keystrokes in the form.

class NameForm extends React.Component {
  constructor(props) {
    super(props);
    this.state = {value: ''};

    this.handleChange = this.handleChange.bind(this);
    this.handleSubmit = this.handleSubmit.bind(this);
  }

  handleChange(event) {
    this.setState({value: event.target.value});
  }

  handleSubmit(event) {
    alert('A name was submitted: ' + this.state.value);
    event.preventDefault();
  }

  render() {
    return (
      <form onSubmit={this.handleSubmit}>
        <label>
          Name:
          <input type="text" value={this.state.value} onChange={this.handleChange} />
        </label>
        <input type="submit" value="Submit" />
      </form>
    );
  }
}

3. How do we target what the user is entering if we have an event handler on an input field?
      * by utilizing 'this.state.value' in both the input field and the handle change function. onChange={this.handleChange} is the line of code that montiors changes to the input field.

## [The Conditional (Ternary) Operator Explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)

1. Why would we use a ternary operator?
      * cleaner shorter code. 
      // WTF 
      What condition ? value if true : value if false
2. Rewrite the following statement using a ternary statement:
let x=1
let y=2
x===y ? console.log(true) : console.log(false)

if(x===y){
  console.log(true);
} else {
  console.log(false);
}

## Bookmark and Review

[React Bootstrap - Forms](https://react-bootstrap.github.io/forms/overview/)
[React Docs - conditional rendering](https://reactjs.org/docs/conditional-rendering.html)