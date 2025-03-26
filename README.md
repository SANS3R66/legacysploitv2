# legacysploitv2
another roblox exploit for older version (2021M)

## How does this works
1. getting RBX::TaskScheduler (maybe MK2) singletone
2. getting jobs -> finding RBX::DataModelJob in jobs (RBX::WaitingScriptJob for now)
3. getting RBX::DataModel from RBX::DataModelJob field
4. getting RBX::ScriptContext as RBX::DataModel child
5. getting global lua state from RBX::ScriptContext
6. increasing identity (non implemented)
7. pushing UNC functions (non implemented)
8. wrapping roblox lua_State globals with our lua_State (non implemented)

## How to build
Simply open .sln file in vs2019 (used by me) (you can also open in vs2022)

# TODO's list
- [ ] general exploiting
  - [x] getting DataModel 
  - [x] getting lua_State
  - [ ] fix identity increase
  - [ ] luau wrapper
  - [ ] gui? (ImGui with dxd11hook)

- [ ] roblox lua c api
  - [x] lua_newthread
  - [x] lua_getfield
  - [x] lua_call
  - [ ] lua_pcall
  - [ ] lua_setfield
  - [ ] lua_pushcclosure
  - [ ] lua_pushvalue
  - [ ] lua_pushstring
  - [ ] lua_pushnumber
  - [ ] lua_pushboolean
