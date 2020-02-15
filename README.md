# DHT-1.3.8
This is a copy for [XOD](https://xod.io/) patches of [Adafruit DHT Humidity & Temperature Sensor Library - v1.3.8](https://github.com/adafruit/DHT-sensor-library) **WITHOUT** the Adafruit Unified Sensor Library library in order to reduce the **size** of transpiled *(compiled)* patches for XOD.

How to use in a **XOD patch**:

````
#pragma XOD error_raise enable

#pragma XOD require "https://github.com/as000fm/DHT-1.3.8"

{{#global}}
#include <DHT.h>
{{/global}}

struct State {
};

{{ GENERATED_CODE }}

void evaluate(Context ctx) {
    //auto inValue = getValue<input_IN>(ctx);
    //emitValue<output_OUT>(ctx, inValue);
}
````
