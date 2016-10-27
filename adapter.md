## Adapter 适配器

### 意图



### 适用性

### 示例

```js
import Light from '../../common/Light';
import LightOnCommand from '../../common/LightOnCommand';
import SimpleRemoteControl from '../../common/SimpleRemoteControl';

let oSimpleRemote = new SimpleRemoteControl();
let oLight = new Light();
let oLightCommand = new LightOnCommand(oLight);

oSimpleRemote.setCommand(oLightCommand);
oSimpleRemote.buttonWasPressed();
```