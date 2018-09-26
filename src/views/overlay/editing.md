<<<<<<< HEAD
/**
 *@title：设置线、面可编辑
 */

=======
>>>>>>> upstream/master
import React, { Component } from 'react';
import ReactDOM from 'react-dom';
import {
  Map, Polygon, Polyline,
} from 'rc-bmap';
import { Button } from 'antd';

class Example extends Component {
  constructor(props) {
    super(props);
    this.state = {
<<<<<<< HEAD
      polyline: {
        points: [
          {
            lng: 116.399,
            lat: 39.910,
          },
          {
            lng: 116.405,
            lat: 39.920,
          },
          {
            lng: 116.425,
            lat: 39.900,
          },
        ],
        strokeColor: 'blue',
        strokeWeight: 2,
        strokeOpacity: 0.5,
      },
      polygon: {
        points: [
          {
            lng: 116.387112,
            lat: 39.920977,
          }, {
            lng: 116.385243,
            lat: 39.913063,
          },
          {
            lng: 116.394226,
            lat: 39.917988,
          },
          {
            lng: 116.401772,
            lat: 39.921364,
          },
          {
            lng: 116.41248,
            lat: 39.927893,
          },
        ],
        strokeColor: 'blue',
        strokeWeight: 2,
        strokeOpacity: 0.5,
      },
=======
      center: {
        lng: 116.404,
        lat: 39.915,
      },
      polylinePoints: [
        {
          lng: 116.399,
          lat: 39.910,
        },
        {
          lng: 116.405,
          lat: 39.920,
        },
        {
          lng: 116.425,
          lat: 39.900,
        },
      ],
      polygonPoints: [
        {
          lng: 116.387112,
          lat: 39.920977,
        }, {
          lng: 116.385243,
          lat: 39.913063,
        },
        {
          lng: 116.394226,
          lat: 39.917988,
        },
        {
          lng: 116.401772,
          lat: 39.921364,
        },
        {
          lng: 116.41248,
          lat: 39.927893,
        },
      ],
>>>>>>> upstream/master
      editing: false,
    };
  }

<<<<<<< HEAD
  enableEditing = () => {
=======
  handleEnable = () => {
>>>>>>> upstream/master
    this.setState({
      editing: true,
    });
  }

<<<<<<< HEAD
  disableEditing = () => {
=======
  handleDisable = () => {
>>>>>>> upstream/master
    this.setState({
      editing: false,
    });
  }

  render() {
    const {
<<<<<<< HEAD
      polyline, polygon, editing,
=======
      center, polylinePoints, polygonPoints, editing,
>>>>>>> upstream/master
    } = this.state;
    return (
      <div style={{ height: '90vh' }}>
        <Map
<<<<<<< HEAD
          ak="dbLUj1nQTvDvKXkov5fhnH5HIE88RUEO"
=======
          ak="WAeVpuoSBH4NswS30GNbCRrlsmdGB5Gv"
          center={center}
          zoom={15}
>>>>>>> upstream/master
          scrollWheelZoom
        >

          <Polyline
<<<<<<< HEAD
            points={polyline.points}
            strokeColor={polyline.strokeColor}
            strokeWeight={polyline.strokeWeight}
            strokeOpacity={polyline.strokeOpacity}
            editing={editing}
          />
          <Polygon
            points={polygon.points}
            strokeColor={polygon.strokeColor}
            strokeWeight={polygon.strokeWeight}
            strokeOpacity={polygon.strokeOpacity}
            editing={editing}
          />
        </Map>
        <Button onClick={this.enableEditing}>开启线、面编辑功能</Button>
        <Button onClick={this.disableEditing}>关闭线、面编辑功能</Button>
=======
            points={polylinePoints}
            strokeColor="blue"
            strokeWeight={2}
            strokeOpacity={0.5}
            editing={editing}
          />
          <Polygon
            points={polygonPoints}
            strokeColor="blue"
            strokeWeight={2}
            strokeOpacity={0.5}
            editing={editing}
          />
        </Map>
        <Button onClick={this.handleEnable}>开启线、面编辑功能</Button>
        <Button onClick={this.handleDisable}>关闭线、面编辑功能</Button>
>>>>>>> upstream/master
      </div>
    );
  }
}

ReactDOM.render(
  <Example />,
  document.getElementById('root'),
);
