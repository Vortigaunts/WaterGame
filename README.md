Let's make a game!
	name: Hydration clicker
Layout
	use default
Settings
	use default

Buttons
	*waterButton
		name:Take a sip
		on click:yield 1 water
	
Resources
	*water
		name:Water
		desc:You've got to drink something

Buildings
	*puddle|puddles
		name:Puddle|Puddles
		desc:A small collection of rainwater
		cost:5 water
		on tick:yield 1 water
		unlocked

Upgrades
	*cupOfWater
		name:A tall glass of water
		desc:Theres nothing more refreshing... increase water gained by taking a sip
		cost:10 water
		passive:increase water yield of waterButton by 2
		
