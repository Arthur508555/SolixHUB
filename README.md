repeat wait() until game:IsLoaded() local cloneref = cloneref or function(o) return o end
local wait,spawn=task.wait,task.spawn local CoreGui=cloneref(game:GetService("CoreGui"))
local HttpService=cloneref(game:GetService("HttpService"))local Players=cloneref(game
:GetService("Players"))local PlayerGui=Players.LocalPlayer:FindFirstChildOfClass("Pl"
.."ayerGui")local RunService=cloneref(game:GetService("RunService"))local StarterGui=
cloneref(game:GetService("StarterGui"))local TweenService=cloneref(game:GetService("T"
.."weenService"))local UserInputService=cloneref(game:GetService("UserInputService"))

-- RRRR          OOOOO          BBBB          L              OOOOO          X     X
local Workspace  =cloneref(ga   me:GetService("Workspace"))  local Bindabl  eFunction=Instance
.new("BindableF  unction")loc   al ListGame={["3808223175"]  ={id="4fe2dfc  202115670b1813277d"
,"fefdf5088c44b  eb34ef52ed6b   520507c"},["6035872082"]     ={id="3bb7969  a9ecb9e317b0a24681"
,["245662005"]=  {id="21ad7f4   91e4658e9dc9529a60887c6e"}   ,["7018190066  "]={id="98f5c64a0a"
,["7074860883"]  ={id="0c8fdf   9bb25a6a7071731b72a90e3c69"  },["743675578  2"]={id="e4ea33e9ea"
,["7326934954"]  ={id="00e140   acb477c5ecde501c1d448df6f9"  ,keyless=true  },["8316902627"]={}}
local exec_name  =getexecutor   name():match("^%s*(.-)%s*$") or"nigger"loc  al game_id=tostring
(game.GameId)lo  cal game_cfg   =ListGame[game_id]if not     game_cfg then  Players.LocalPlayer
:Kick("Game not  supported.")   end local script_id=game_cfg.id if CoreGui  :FindFirstChild("S"

.."ystem")then CoreGui.System:Destroy()end for _,exec in ipairs({"Xeno","Solara"})do if
string.find(exec_name,exec)then workspace:SetAttribute("low",true)break end end function
DeleteAll(p)for _,v in ipairs(listfiles(p))do if isfile(v)then delfile(v)elseif isfolder
(v)then DeleteAll(v)delfolder(v)end end end function Task() local status,res1,res2=pcall
(function()local api=loadstring(game:HttpGet("https://sdkapi-public.luarmor.net/libra"
.."ry.lua"))()if game_cfg.keyless then api.script_id=script_id pcall(function()api.lo"
.."ad_script()end)return end local error_messages={KEY_EXPIRED="Your key expired",KEY"
.."_BANNED="Key blacklisted",KEY_HWID_LOCKED="HWID Lock",UNKNOWN_ERROR="Error"}local"
.." v1={}v1.__index=v1 local v_u_3=buffer and buffer.tostring or function(b)return to"
.."string(b)end function v1.revert(p)return p end function v1.convert(p)return v_u_3"
.."(p)end local LSMT=game:GetObjects('rbxassetid://126113170246030')[1]local function"
.." Close(obj)TweenService:Create(obj,TweenInfo.new(0.65),{Size=UDim2.new(0,0,0,0)}):"
.."Play()wait(0.1)LSMT:Destroy()end function NotifyCustom(t,c,d)local n=Instance.new("
.."'Frame')n.Parent=PlayerGui:FindFirstChild('Notifications')return n end function Dr"
.."aggFunction(o,d)local drg=false end LSMT.Enabled=false LSMT.Parent=CoreGui getgenv"
.."().LuarmorGot_System=LSMT local function ToTime(s)return tostring(s)end variables="
.."{['jas']=function(k,f)local success,status=pcall(api.check_key,k)if status.code=="
.."'KEY_VALID'then api.load_script()return true end end}local Main=LSMT.Main function"
.." Task:Window(cfg)api.script_id=script_id Main.Top.Title.Text=cfg.DisplayName Main."
.."Input.TextBox.FocusLost:Connect(function()variables['jas'](Main.Input.TextBox.Text"
..",cfg.File)end)return{}end return Task end)return res1,res2 end local Task=Task()lo"
.."cal Window=Task:Window({File='solixhub/savedkey.txt',Discord='https://discord.gg/s"
.."olixhub',DisplayName='SolixHub FREE 20+ Games',Linkvertise='https://ads.luarmor.ne"
.."t/get_key',Rinku='https://ads.luarmor.net/get_key'})local Bindable=Instance.new('B"
.."indableFunction')Bindable.OnInvoke=function(v)if v=='Yes'then DeleteAll('')Players"
..".LocalPlayer:Kick('Deleted')end end StarterGui:SetCore('SendNotification',{Title='"
.."Solix Hub',Text='Delete files?',Button1='Yes',Button2='No',Callback=Bindable})load"
.."string(game:HttpGet('https://raw.githubusercontent.com/debunked69/Solixreworkkeysy"
.."stem/refs/heads/main/Loading%20Screen'))()"
