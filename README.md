### ethereum-ruby
---
https://github.com/DigixGlobal/ethereum-ruby

```rb
gem 'ethereum'

client = Ethereum::IpcClient.new("#{ENV['HOME']}/.ethereum_testnet/geth.ipc")

init = Ethereum::Initializer.new("#{ENV['PWD']}/spec/fixxtures/SimpleNameRegistry.sol", client)
init.build_all
simple_name_registry_instance = SimpleNameRegistry.new
simple_name_registry_instance.deploy_and_wait(60)

transact_[function_name](params)
transact_and_wait_[function_name](params)
call_[function_name](params)

contract SimpleNameRegistry {
  
  mapping (address => bool) public myMapping;
  
  function register(address _a, bytes32 _b) {
  }
  
  function getSomeValue(address _x) public constant returns(bool b, address b) {
  }
}

simple_name_registry_instance.transact_and_wait_register("", "minter.contact.dgx")
simple_name_registry_instance.transact_register("", "anthony@eufemio.dgx")
simple_name_registry_instance.call_get_some_value("xxx")
simple_name_resistry_instance.call_my_mapping("xxx")

simple_name_registry_instance.as("xxx")

```

```sh
bundle
gem install ethereum
```

```
```


