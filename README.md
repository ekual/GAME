	
	public function processInput()
	{
		var _loc_1:* = getTimer() - this.lastFrameTime;
		if (_loc_1 == 0)
		{
			return;
		}
		this.lastFrameTime = this.lastFrameTime + _loc_1;
		if (_loc_1 > 100)
		{
			_loc_1 = 100;
		}
		_loc_1 = _loc_1 / 1000;
		rotateObject(_loc_1);
		getDisplacement(_loc_1);
		applyDisplacement();
	}
	public function rotateObject(t:Number):void
	{
			if (Eventos.keyDe){ rot += 100 * t; }
			if (Eventos.keyIz){ rot -= 100 * t; }
	}
	public function getDisplacement(t:Number):void
	{
		if (Eventos.keyW) { pos.x += speed * t; }
		if (Eventos.keyS) { pos.x -= speed * t; }

		if (Eventos.keyA) { pos.z -= speed * t; }
		if (Eventos.keyD) { pos.z += speed * t; }
	}
	public function applyDisplacement():void
	{
		GAME.setPos(pos,rot);
		GAME.update();
	}
	
	
	
}
