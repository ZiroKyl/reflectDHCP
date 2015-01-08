# Reflect helpers for [krolaw/dhcp4](https://github.com/krolaw/dhcp4)
This package adds simple way to init DHCP4 Options from JSON object. For example, read DHCP Options from JSON formatted config file.

Born from [this](https://github.com/krolaw/dhcp4/pull/9) Pull Request.

## Usage
```go
import "encoding/json"
import "github.com/krolaw/dhcp4"
import "github.com/ZiroKyl/reflectDHCP"
...
var opt = dhcp4.Options{};
json.Unmarshal(strJSON, (*reflectDHCP.Options)(&opt));
```
For more examples see [test file](https://github.com/ZiroKyl/reflectDHCP/blob/master/OptionsHelper_test.go#L181)
