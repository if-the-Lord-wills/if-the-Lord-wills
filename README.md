repeat
	if the_Lord.wills then
		task.defer(action.next)
	else
		break
	end
until life.end
