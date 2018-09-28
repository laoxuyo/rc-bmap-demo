import React from 'react';
import ReactDOM from 'react-dom';
import {
  Map,
  ControlAnchor,
  CopyrightControl,
  Copyright,
} from 'rc-bmap';

class Example extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      center: {
        lng: 116.404,
        lat: 39.915,
      },
    };
  }

  render() {
    const {
      center,
      content
    } = this.state;
    return ( 
      <div style = {{height: '100vh'}} > 
      我是自定义版权控件呀
      </div>
    );
  }
}

ReactDOM.render(<Example />, document.getElementById('root'), );