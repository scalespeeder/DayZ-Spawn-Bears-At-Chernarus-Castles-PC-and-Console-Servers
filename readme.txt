DayZ "Bears Spawn At Castles" XML Mod For Consoles & PC XML Snippets Instructions & Terms Of Use

These snippets will spawn in the Bears ( Animal_UrsusArctos ) at various Castles & Castle Ruins around Chernarus

Please note the instructions at the end of this readme, which tell you to comment out the non-Castle Bear territories if you want Bears to only spawn at Castles.

WARNING! THESE BEARS ARE VERY DIFFICULT TO KILL!!!!!

Limited Testing on PC Chernarus Local Server DAYZ Version 1.20 Mar 2023.

XML Snippets Created by @scalespeeder. Please report bugs & errors to scalespeeder@gmail.com with screenshots.

TERMS OF USE
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS
OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN
AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH
THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Using these modded xml / json files and instructions could break the functioning of your DAYZ server, requiring a reinstall that would wipe
all player progress.

Using these modded files neccessitates increased regular restarts to prevent server crashing.

It is suggested you thoroughly test your server after applying these files to ensure proper
functioning of your server.

I always recomend you validate your files at: https://www.xmlvalidation.com/ and https://jsonformatter.curiousconcept.com/

Instructions:
	
This code snippet should be inserted into your events.xml file, replacing the AnimalBear entry :
	
	<!-- Bears at castle events entry-->
	
	    <event name="AnimalBear">
        <nominal>0</nominal>
        <min>11</min><!--vanilla is 2-->
        <max>11</max><!--vanilla is 2-->
        <lifetime>180</lifetime>
        <restock>0</restock>
        <saferadius>200</saferadius>
        <distanceradius>0</distanceradius>
        <cleanupradius>0</cleanupradius>
        <flags deletable="0" init_random="0" remove_damaged="1"/>
        <position>fixed</position>
        <limit>custom</limit>
        <active>1</active>
        <children>
            <child lootmax="0" lootmin="0" max="1" min="1" type="Animal_UrsusArctos"/><!--vaniila is max="1" min="1" -->
        </children>
    </event>
	
	<!-- Bears at castle end -->
	
	
Add this code snippet to your bear_territories.xml, at the top, under <territory-type> :

<!-- Bears at castles territories entry-->

 <territory color="4294923520">
        <zone name="Graze" 	smin="0" smax="0" dmin="0" dmax="0" x="6554.89" z="5612.14" r="60"/> 
		</territory>
		<territory color="4294923520">
        <zone name="Graze" 	smin="0" smax="0" dmin="0" dmax="0" x="6913.05" z="11376.50" r="140"/>
		</territory>
		<territory color="4294923520">
        <zone name="Graze" 	smin="0" smax="0" dmin="0" dmax="0" x="6879.56" z="11491.69" r="120"/>
		</territory>
		<territory color="4294923520">
        <zone name="Graze" 	smin="0" smax="0" dmin="0" dmax="0" x="10278.76" z="12053.40" r="70"/>  
		</territory>
		<territory color="4294923520">
        <zone name="Graze" 	smin="0" smax="0" dmin="0" dmax="0" x="1417.17" z="9258.70" r="120"/> 
		</territory>
		<territory color="4294923520">
        <zone name="Graze" 	smin="0" smax="0" dmin="0" dmax="0" x="1437.84" z="9221.45" r="70"/>
		</territory>
		<territory color="4294923520">
		<zone name="Graze" 	smin="0" smax="0" dmin="0" dmax="0" x="13497.35" z="3301.73" r="140"/>
		</territory>
		<territory color="4294923520">
        <zone name="Graze" 	smin="0" smax="0" dmin="0" dmax="0" x="13422.18" z="3287.93" r="120"/> 
		</territory>
		<territory color="4294923520">
        <zone name="Graze" 	smin="0" smax="0" dmin="0" dmax="0" x="11246.05" z="4295.07" r="70"/> 
		</territory>
		<territory color="4294923520">
        <zone name="Graze" 	smin="0" smax="0" dmin="0" dmax="0" x="9302.82" z="13506.66" r="120"/> 
		</territory>
		<territory color="4294923520">
        <zone name="Graze" 	smin="0" smax="0" dmin="0" dmax="0" x="7418.32" z="9115.28" r="70"/>  
</territory>


<!-- Bears at castles end -->


If you want the Bears to only spawn at the Castles, comment out the rest of the territories using arrow brackets



	
Save and re-upload if necessary and re-start your server for the changes to take effect.

Thanks, Rob.