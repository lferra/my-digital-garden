---
{"dg-publish":true,"permalink":"/script-rework/","dgHomeLink":true,"dgPassFrontmatter":false}
---


## Assumptions

1. Every Windows server has to have Cygwin installed
2. All the scheduling is triggered by Crontab / SSH
3. Ideally all the activities (log browsing, script amendment, etc.), are done via 

## Cygwin

1. Install perl package (dependencies perl-base and perl-autobase will be selected automatically)

## Directory

### shl
Contains specific and generic bash scripts

### log
Contains logs, with separated log_acq and log_dsp subdirectories. Each subdirectory has a further spazio subdirectory with the detailed log (/l option of each operation)

### bin
Contains utilities

/pub
fdfsfdfssdffdfd

<style>
.container {font-family: sans-serif; text-align: center;}
.button-wrapper button {z-index: 1;height: 40px; width: 100px; margin: 10px;padding: 5px;}
.excalidraw .App-menu_top .buttonList { display: flex;}
.excalidraw-wrapper { height: 800px; margin: 50px; position: relative;}
:root[dir="ltr"] .excalidraw .layer-ui__wrapper .zen-mode-transition.App-menu_bottom--transition-left {transform: none;}
</style><script src="https://unpkg.com/react@17/umd/react.production.min.js"></script><script src="https://unpkg.com/react-dom@17/umd/react-dom.production.min.js"></script><script type="text/javascript" src="https://unpkg.com/@excalidraw/excalidraw@0.12.0/dist/excalidraw.production.min.js"></script><div id="Drawing_2022-09-07_2249.11.excalidraw.md1"></div><script>(function(){const InitialData={"type":"excalidraw","version":2,"source":"https://excalidraw.com","elements":[{"type":"rectangle","version":16,"versionNonce":404564201,"isDeleted":false,"id":"t80za_11kRh_O1AhP1m7e","fillStyle":"hachure","strokeWidth":1,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-111,"y":-190.5,"strokeColor":"#364fc7","backgroundColor":"#fab005","width":231,"height":105,"seed":1313425607,"groupIds":[],"strokeSharpness":"sharp","boundElements":[],"updated":1662583791556,"link":null,"locked":false},{"type":"ellipse","version":42,"versionNonce":1649735207,"isDeleted":false,"id":"zFQevUabFTT0bxJrj6KLH","fillStyle":"hachure","strokeWidth":1,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-140.5,"y":-97,"strokeColor":"#0b7285","backgroundColor":"#be4bdb","width":147.5,"height":126.5,"seed":2050401097,"groupIds":[],"strokeSharpness":"sharp","boundElements":[],"updated":1662583791556,"link":null,"locked":false},{"type":"freedraw","version":75,"versionNonce":120833735,"isDeleted":false,"id":"FqRB95utWoRAT_FmceTLQ","fillStyle":"hachure","strokeWidth":1,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-74,"y":68.73684210526315,"strokeColor":"#e67700","backgroundColor":"#be4bdb","width":386,"height":262,"seed":1370424521,"groupIds":[],"strokeSharpness":"round","boundElements":[],"updated":1662583833321,"link":null,"locked":false,"points":[[0,0],[-0.5,-1],[-1.4999999999999998,-2],[-5,-32.5],[-5,-60.5],[4,-112.5],[10.5,-137],[35.5,-190.5],[49.5,-211.5],[76,-239],[80,-242],[80.5,-242.5],[80.5,-241],[80.5,-233.5],[75.5,-208.5],[71.5,-185.5],[61,-144],[54.5,-121.5],[37,-63.5],[34.5,-52.5],[34,-40.5],[34,-38],[34,-37.5],[34,-37],[35.5,-38],[59,-53.5],[111,-104],[138.5,-132.5],[195.5,-184.5],[225.5,-208],[279,-244.5],[295.5,-255.5],[295.5,-254],[293.5,-251],[291,-240],[284,-217.5],[278,-198],[270,-177],[246.5,-130.5],[236.5,-107],[223.5,-82.5],[204,-41],[197.5,-25.5],[186,-1],[183.5,5.5],[183.5,6.5],[186,4],[205.5,-25.5],[218.5,-46.5],[264,-100],[293,-124.5],[346,-159.5],[368,-171.5],[381,-178.5],[380,-177.5],[372.5,-168.5],[362,-158.5],[338.5,-144],[270,-118.5],[236,-112],[170,-104.5],[137.5,-102],[107.5,-100.5],[36.5,-91.5],[23.5,-89],[9.5,-86.5],[6,-85],[3.5,-84.5],[3,-84.5],[2,-84.5],[2,-84],[2,-84]],"lastCommittedPoint":null,"simulatePressure":true,"pressures":[]},{"type":"text","version":26,"versionNonce":1263639346,"isDeleted":false,"id":"D6v7X8Py","fillStyle":"hachure","strokeWidth":1,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-48,"y":37.73684210526312,"strokeColor":"#000000","backgroundColor":"#be4bdb","width":144,"height":25,"seed":800690375,"groupIds":[],"strokeSharpness":"sharp","boundElements":[],"updated":1662856095768,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"AAAAAASSSSD","rawText":"AAAAAASSSSD","baseline":18,"textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"AAAAAASSSSD"},{"type":"text","version":39,"versionNonce":1444424814,"isDeleted":false,"id":"rvViiP3Q","fillStyle":"hachure","strokeWidth":1,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":-56,"y":-163,"strokeColor":"#5f3dc4","backgroundColor":"#be4bdb","width":123,"height":25,"seed":736942183,"groupIds":[],"strokeSharpness":"sharp","boundElements":[],"updated":1662856092517,"link":null,"locked":false,"fontSize":20,"fontFamily":1,"text":"SSSSSSSSSS","rawText":"SSSSSSSSSS","baseline":18,"textAlign":"left","verticalAlign":"top","containerId":null,"originalText":"SSSSSSSSSS"},{"type":"diamond","version":73,"versionNonce":1795495474,"isDeleted":false,"id":"wWR9FQLcuJPFdQxsL0L0s","fillStyle":"hachure","strokeWidth":1,"strokeStyle":"solid","roughness":1,"opacity":100,"angle":0,"x":32.643939393939405,"y":-132.78309409888354,"strokeColor":"#d9480f","backgroundColor":"#4c6ef5","width":206.66666666666666,"height":174.84848484848484,"seed":1872922418,"groupIds":[],"strokeSharpness":"sharp","boundElements":[],"updated":1662852901725,"link":null,"locked":false},{"id":"niRBihBTbsolCw4900Yt6","type":"rectangle","x":25.371212121212125,"y":13.88357256778312,"width":169.09090909090907,"height":89.09090909090907,"angle":0,"strokeColor":"#5c940d","backgroundColor":"#868e96","fillStyle":"hachure","strokeWidth":1,"strokeStyle":"solid","roughness":1,"opacity":100,"groupIds":[],"strokeSharpness":"sharp","seed":9332974,"version":48,"versionNonce":1647060274,"isDeleted":false,"boundElements":null,"updated":1662856685102,"link":null,"locked":false}],"appState":{"theme":"dark","viewBackgroundColor":"#ffffff","currentItemStrokeColor":"#5c940d","currentItemBackgroundColor":"#868e96","currentItemFillStyle":"hachure","currentItemStrokeWidth":1,"currentItemStrokeStyle":"solid","currentItemRoughness":1,"currentItemOpacity":100,"currentItemFontFamily":1,"currentItemFontSize":20,"currentItemTextAlign":"left","currentItemStrokeSharpness":"sharp","currentItemStartArrowhead":null,"currentItemEndArrowhead":"arrow","currentItemLinearStrokeSharpness":"round","gridSize":null,"colorPalette":{}},"files":{}};InitialData.scrollToContent=true;App=()=>{const e=React.useRef(null),t=React.useRef(null),[n,i]=React.useState({width:void 0,height:void 0});return React.useEffect(()=>{i({width:t.current.getBoundingClientRect().width,height:t.current.getBoundingClientRect().height});const e=()=>{i({width:t.current.getBoundingClientRect().width,height:t.current.getBoundingClientRect().height})};return window.addEventListener("resize",e),()=>window.removeEventListener("resize",e)},[t]),React.createElement(React.Fragment,null,React.createElement("div",{className:"excalidraw-wrapper",ref:t},React.createElement(ExcalidrawLib.Excalidraw,{ref:e,width:n.width,height:n.height,initialData:InitialData,viewModeEnabled:!0,zenModeEnabled:!0,gridModeEnabled:!1})))},excalidrawWrapper=document.getElementById("Drawing_2022-09-07_2249.11.excalidraw.md1");ReactDOM.render(React.createElement(App),excalidrawWrapper);})();</script>

blah blah
