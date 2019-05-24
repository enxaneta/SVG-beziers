<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Distance along an SVG path to a given point</title>
<style>
      
svg{border:1px solid;stroke-width:3px;pointer-events:stroke;}
path {
  fill: none;
  stroke: black; 
}

path:hover{cursor:pointer;}
    </style>
</head>

<body>

<svg id="svg" viewBox="40 30 370 370" width="500">
<path id="thePath" d="M217.72860717773438,308.86431884765625C86.77467662487854,313.7806863748062 47.01987177713832,205.63816674597538 127.13864135742188,124.95574951171875 C170.7964630126953,85.6637191772461 152.24188232421875,234.64601135253906 326.3274230957031,112.9498519897461 C407.8219755446947,58.75656029439313 377.6253662109375,302.8613586425781 217.72860717773438,308.86431884765625 z"></path>
<circle fill="red" r="7" id="mark" />
<circle fill="gold" r="4" id="test" />
</svg>

<script>
const SVG_NS = "http://www.w3.org/2000/svg";
//I have the coordinates of a point somewhere along an SVGPath.
let pointPos = { x: 91.8, y: 245.44 };
//Just for the demo:
//setting the cx and cy of the red circle: a circle to mark the position of the point
updateElement({ cx: pointPos.x, cy: pointPos.y }, mark);


//the function used to get the distance along the path to the point

function getLengthAtPoint(point, path) {
  //the total length of the path
  let pathLength = thePath.getTotalLength();
  // if precision = 100:: the path is divided in 100 segments
  let precision = 100;
  //the length of each segment is:
  let division = pathLength / precision;
  let threshold = 1;
  let theRecord = pathLength;
  let theSegment;
  let theDistance;

  for (let i = 0; i < precision; i++) {
    // a point on the path
    let p = thePath.getPointAtLength(i * division);
    // the distance between the point position and p
    theDistance = dist(pointPos, p);
    //I'm searching for the smallest distance between point position and p
    if (theDistance < theRecord) {
      theSegment = i;
      theRecord = theDistance;
    }
    //if the distance is smaller than the threshold (1) break the loop. No need to search anylonger
    if (theDistance < threshold) {
      break;
    }
  }
  //get the distance along the path to this point
  return theSegment * division + theDistance;
}


//call the function to get the distance
let D = getLengthAtPoint(pointPos, thePath);

// Test it:
let testPoint = thePath.getPointAtLength(D);
// update the position of the golden circle
updateElement({ cx: testPoint.x, cy: testPoint.y }, test);

function updateElement(o, element) {
  for (var name in o) {
    if (o.hasOwnProperty(name)) {
      element.setAttributeNS(null, name, o[name]);
    }
  }
  return element;
}

function dist(p1, p2) {
  let dx = p2.x - p1.x;
  let dy = p2.y - p1.y;
  return Math.sqrt(dx * dx + dy * dy);
}
</script>

</body>
</html>
