local life = require("life")
local action = require("action")

local function main()
	repeat
		if the_Lord.wills then
			task.spawn(action.immediate)
			task.spawn(action.prayer)
			task.defer(action.next)
		else
			break
		end
	until life.finished
	return 1
end
