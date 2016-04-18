# Minecraft_Ravine

ravine = function(){
	
	var myDrone = new Drone (self);

	myDrone.down(40).box(0, 20, 70, 120);

	myDrone.move("start");
    
    myDrone.down(40).box(20, 20, 1, 120);
    
    myDrone.move("start");
    
    for (var Air=0; Air < 150; Air++){
       var distanceX = parseInt(20 * Math.random() );
       var distanceZ = parseInt(120 * Math.random() );
       var blockY = parseInt(Math.random() * 8);
       myDrone.down(40).fwd(distanceZ).right(distanceX).box(0);
       myDrone.move("start");
       
       
   } ;
    
    for (var lavaDrip=0; lavaDrip < 80; lavaDrip++){
       var distanceX = parseInt(20 * Math.random() );
       var distanceZ = parseInt(120 * Math.random() );
       var blockY = parseInt(Math.random() * 8);
       myDrone.down(30).fwd(distanceZ).right(distanceX).box(11);
       myDrone.move("start");
       
       
   } ;
}
exports.ravine = ravine;
