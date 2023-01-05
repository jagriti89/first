# first
import React from 'react';
class App extends React.Component{
    constructor(props){
    super(props);
    this.state={
        count:1,
    };}

    render(){
        return (
            <div>
                <h1> Assignent </h1>
                <div>
                    Counter: {this.state.count}
                    <br></br><br></br>
                    <button  onClick={() => {
                        this.setState({
                        count: this.state.count -1,
                        })           
                    }}>click me decrease</button>,<br></br><br></br>
                    <button onClick={()=>{
                        this.setState({
                            count:this.state.count +1
                        } )
                    }}>click me increase </button>
                </div>
                
            </div>
        );
    }
}
export default App;
