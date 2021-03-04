# Simple-Bash-Scripts
A collection of bash scripts.

<!DOCTYPE html><html lang="en-US" prefix="og: http://ogp.me/ns# fb: http://ogp.me/ns/fb#"><head><meta charset="UTF-8"/>
<script data-ezscrex='false' data-cfasync='false' data-pagespeed-no-defer>var __ez=__ez||{};__ez.stms=Date.now();__ez.evt={};__ez.script={};__ez.ck=__ez.ck||{};__ez.template={};__ez.template.isOrig=false;__ez.queue=(function(){var count=0,incr=0,items=[],timeDelayFired=false,hpItems=[],lpItems=[],allowLoad=true;var obj={func:function(name,funcName,parameters,isBlock,blockedBy,deleteWhenComplete,proceedIfError){var self=this;this.name=name;this.funcName=funcName;this.parameters=parameters===null?null:(parameters instanceof Array)?parameters:[parameters];this.isBlock=isBlock;this.blockedBy=blockedBy;this.deleteWhenComplete=deleteWhenComplete;this.isError=false;this.isComplete=false;this.isInitialized=false;this.proceedIfError=proceedIfError;this.isTimeDelay=false;this.process=function(){log("... func = "+name);self.isInitialized=true;self.isComplete=true;log("... func.apply: "+name);var funcs=self.funcName.split('.');var func=null;if(funcs.length>3){}else if(funcs.length===3){func=window[funcs[0]][funcs[1]][funcs[2]];}else if(funcs.length===2){func=window[funcs[0]][funcs[1]];}else{func=window[self.funcName];}
if(typeof func!=='undefined'&&func!==null){func.apply(null,this.parameters);}
if(self.deleteWhenComplete===true)delete items[name];if(self.isBlock===true){log("----- F'D: "+self.name);processAll();}}},file:function(name,path,isBlock,blockedBy,async,defer,proceedIfError){var self=this;this.name=name;this.path=path;this.async=async;this.defer=defer;this.isBlock=isBlock;this.blockedBy=blockedBy;this.isInitialized=false;this.isError=false;this.isComplete=false;this.proceedIfError=proceedIfError;this.isTimeDelay=false;this.process=function(){self.isInitialized=true;log("... file = "+name);var scr=document.createElement('script');scr.src=path;if(async===true)scr.async=true;else if(defer===true)scr.defer=true;scr.onerror=function(){log("----- ERR'D: "+self.name);self.isError=true;if(self.isBlock===true){processAll();}};scr.onreadystatechange=scr.onload=function(){var state=scr.readyState;log("----- F'D: "+self.name);if((!state||/loaded|complete/.test(state))){self.isComplete=true;if(self.isBlock===true){processAll();}}};document.getElementsByTagName('head')[0].appendChild(scr);}}};function init(){window.addEventListener("load",function(){setTimeout(function(){timeDelayFired=true;log('TDELAY -----');processAll();},5000);},false);}
function addFile(name,path,isBlock,blockedBy,async,defer,proceedIfError,priority){var item=new obj.file(name,path,isBlock,blockedBy,async,defer,proceedIfError);if(priority===true){hpItems[name]=item}else{lpItems[name]=item}
items[name]=item;checkIfBlocked(item);}
function setallowLoad(settobool){allowLoad=settobool}
function addFunc(name,func,parameters,isBlock,blockedBy,autoInc,deleteWhenComplete,proceedIfError,priority){if(autoInc===true)name=name+"_"+incr++;var item=new obj.func(name,func,parameters,isBlock,blockedBy,deleteWhenComplete,proceedIfError);if(priority===true){hpItems[name]=item}else{lpItems[name]=item}
items[name]=item;checkIfBlocked(item);}
function addTimeDelayFile(name,path){var item=new obj.file(name,path,false,[],false,false,true);item.isTimeDelay=true;log(name+' ... '+' FILE! TDELAY');lpItems[name]=item;items[name]=item;checkIfBlocked(item);}
function addTimeDelayFunc(name,func,parameters){var item=new obj.func(name,func,parameters,false,[],true,true);item.isTimeDelay=true;log(name+' ... '+' FUNCTION! TDELAY');lpItems[name]=item;items[name]=item;checkIfBlocked(item);}
function checkIfBlocked(item){if(isBlocked(item)===true||allowLoad==false)return;item.process();}
function isBlocked(item){if(item.isTimeDelay===true&&timeDelayFired===false){log(item.name+" blocked = TIME DELAY!");return true;}
if(item.blockedBy instanceof Array){for(var i=0;i<item.blockedBy.length;i++){var block=item.blockedBy[i];if(items.hasOwnProperty(block)===false){log(item.name+" blocked = "+block);return true;}else if(item.proceedIfError===true&&items[block].isError===true){return false;}else if(items[block].isComplete===false){log(item.name+" blocked = "+block);return true;}}}
return false;}
function log(msg){var href=window.location.href;var reg=new RegExp('[?&]ezq=([^&#]*)','i');var string=reg.exec(href);var res=string?string[1]:null;if(res==="1")console.debug(msg);}
function processAll(){count++;if(count>200)return;log("let's go");processItems(hpItems);processItems(lpItems);}
function processItems(list){for(var i in list){if(list.hasOwnProperty(i)===false)continue;var item=list[i];if(item.isComplete===true||isBlocked(item)||item.isInitialized===true||item.isError===true){if(item.isError===true){log(item.name+': error')}else if(item.isComplete===true){log(item.name+': complete already')}else if(item.isInitialized===true){log(item.name+': initialized already')}}else{item.process();}}}
init();return{addFile:addFile,addDelayFile:addTimeDelayFile,addFunc:addFunc,addDelayFunc:addTimeDelayFunc,items:items,processAll:processAll,setallowLoad:setallowLoad};})();__ez.evt.add=function(e,t,n){e.addEventListener?e.addEventListener(t,n,!1):e.attachEvent?e.attachEvent("on"+t,n):e["on"+t]=n()},__ez.evt.remove=function(e,t,n){e.removeEventListener?e.removeEventListener(t,n,!1):e.detachEvent?e.detachEvent("on"+t,n):delete e["on"+t]};__ez.script.add=function(e){var t=document.createElement("script");t.src=e,t.async=!0,t.type="text/javascript",document.getElementsByTagName("head")[0].appendChild(t)};__ez.dot={};__ez.queue.addFile('/detroitchicago/boise.js', '/detroitchicago/boise.js?gcb=192-3&cb=1', false, [], true, false, true, false);</script>
<script>var __sellerid="92a6db08b43e2ef47ed9427cb6e2953f";</script>
<link href="//ad.doubleclick.net" rel="dns-prefetch">
<link href="//pagead2.googlesyndication.com" rel="dns-prefetch">
<link href="//googleads.g.doubleclick.net" rel="dns-prefetch">
<link href="//tpc.googlesyndication.com" rel="dns-prefetch">
<link href="//adservice.google.com" rel="dns-prefetch">
<link href="//secureads.g.doubleclick.net" rel="dns-prefetch">
<link href="//www.googletagservices.com" rel="dns-prefetch">
<script data-ezscrex="false" data-cfasync="false" data-pagespeed-no-defer type='text/javascript' id='bsaihudashidsadhu'>window.ezogtk="";if(typeof processGoogleToken!=="function"){processGoogleToken=function(a){window.ezogtk=a.newToken;processGoogleToken=undefined;var el=document.getElementById('bsaihudashidsadhu');if(el!==null){el.parentNode.removeChild(document.getElementById('bsaihudashidsadhu'))}
var eel=document.getElementById('ezintegrator');if(eel!==null){eel.parentNode.removeChild(document.getElementById('ezintegrator'))}}}</script>
<script async="" src="//c.amazon-adsystem.com/aax2/apstag.js"></script>
<script data-cfasync="false" type="text/javascript" data-pagespeed-no-defer>var __ezaps=[{slotID:'div-gpt-ad-thewindowsclub_com-box-3-0',slotName:'/1254144/thewindowsclub_com-box-3',sizes:[[300,250]]},{slotID:'div-gpt-ad-thewindowsclub_com-medrectangle-3-0',slotName:'/1254144/thewindowsclub_com-medrectangle-3',sizes:[[580,400],[336,280],[300,250]]},{slotID:'div-gpt-ad-thewindowsclub_com-banner-2-0',slotName:'/1254144/thewindowsclub_com-banner-2',sizes:[[300,600],[160,600]]},{slotID:'div-gpt-ad-thewindowsclub_com-box-1-0',slotName:'/1254144/thewindowsclub_com-box-1',sizes:[[336,280],[300,250]]},{slotID:'div-gpt-ad-thewindowsclub_com-large-mobile-banner-1-0',slotName:'/1254144/thewindowsclub_com-large-mobile-banner-1',sizes:[[580,400],[336,280],[300,250]]},{slotID:'div-gpt-ad-thewindowsclub_com-medrectangle-1-0',slotName:'/1254144/thewindowsclub_com-medrectangle-1',sizes:[[728,90]]},{slotID:'div-gpt-ad-thewindowsclub_com-box-2-0',slotName:'/1254144/thewindowsclub_com-box-2',sizes:[[728,90]]}];var __ezapid="aa05931b-5308-4ea3-95a2-adf84f4ffde4";!function(a9,a){if(a[a9])return;function q(c,r){a[a9]._Q.push([c,r])}
a[a9]={init:function(){q("i",arguments)},fetchBids:function(){q("f",arguments)},setDisplayBids:function(){},targetingKeys:function(){return[]},_Q:[]};}("apstag",window);apstag.init({pubID:__ezapid,adServer:'googletag',schain:{complete:1,ver:'1.0',nodes:[{asi:'ezoic.ai',sid:__sellerid,hp:1}]}});function ezapsFetchBids(amazonSlots){if(typeof amazonSlots==='undefined'||amazonSlots.length===0){return}
apstag.fetchBids({slots:amazonSlots,timeout:2e3},function(bids){function getSlotById(id){if(typeof window.ezslots==='undefined'||window.ezslots==0){return;}
for(var i=0;i<window.ezslots.length;i++){var slot=window[ezslots[i]];if(typeof slot==='undefined'){continue;}
var slotId=slot.getSlotElementId();if(typeof slotId!=='undefined'&&slotId==id){return slot;}}}
function setA9DisplayBids(bids){if(typeof bids==='undefined'||bids.length==0){return;}
var keys=apstag.targetingKeys();for(var i=0;i<bids.length;i++){var bid=bids[i];var slot=getSlotById(bid.slotID);for(var k=0;k<keys.length;k++){if(keys[k]in bid){slot.setTargeting(keys[k],bid[keys[k]]);}}}}
googletag.cmd.push(function(){setA9DisplayBids(bids);});});}
if(typeof __tcfapi!='undefined'){__tcfapi('addEventListener',2,function(tc,success){if(success&&(tc.eventStatus=="useractioncomplete"||tc.eventStatus=="tcloaded")){if(tc.gdprApplies===false||(("purpose"in tc)&&(tc.purpose.consents["1"]===true)&&("vendor"in tc)&&(tc.vendor.consents["793"]===true))){ezapsFetchBids(__ezaps);}}});}else{ezapsFetchBids(__ezaps);}</script>
<script src="https://adservice.google.com/adsid/integrator.js?domain=www.thewindowsclub.com" id="ezintegrator"></script>
<script type="text/javascript">
	var __banger_pmp_deals=function(){var d={17:{"DealId":17,"Floor":160},18:{"DealId":18,"Floor":25},19:{"DealId":19,"Floor":100},20:{"DealId":20,"Floor":300},21:{"DealId":21,"Floor":2000},22:{"DealId":22,"Floor":2500},23:{"DealId":23,"Floor":3000},24:{"DealId":24,"Floor":4000},25:{"DealId":25,"Floor":5000},26:{"DealId":26,"Floor":6500},601:{"DealId":601,"Floor":13},608:{"DealId":608,"Floor":213},619:{"DealId":619,"Floor":10},760:{"DealId":760,"Floor":99},761:{"DealId":761,"Floor":99},7:{"DealId":7,"Floor":150},8:{"DealId":8,"Floor":200},9:{"DealId":9,"Floor":300},10:{"DealId":10,"Floor":400},11:{"DealId":11,"Floor":500},12:{"DealId":12,"Floor":600},13:{"DealId":13,"Floor":700},14:{"DealId":14,"Floor":800},15:{"DealId":15,"Floor":1000},16:{"DealId":16,"Floor":1500}};return[{"SlotName":"/1254144/thewindowsclub_com-box-2","Deals":[d[17],d[18],d[19],d[20],d[21],d[22],d[23],d[24],d[25],d[26],d[601],d[608],d[619],d[760],d[761],d[7],d[8],d[9],d[10],d[11],d[12],d[13],d[14],d[15],d[16]]},{"SlotName":"/1254144/thewindowsclub_com-box-1","Deals":[d[17],d[18],d[19],d[20],d[21],d[22],d[7],d[8],d[9],d[10],d[11],d[12],d[13],d[14],d[15],d[16]]},{"SlotName":"/1254144/thewindowsclub_com-large-mobile-banner-1","Deals":[d[17],d[18],d[19],d[20],d[7],d[8],d[9],d[10],d[11],d[12],d[13],d[14],d[15],d[16]]},{"SlotName":"/1254144/thewindowsclub_com-medrectangle-3","Deals":[d[17],d[18],d[19],d[20],d[21],d[22],d[23],d[24],d[7],d[8],d[9],d[10],d[11],d[12],d[13],d[14],d[15],d[16]]},{"SlotName":"/1254144/thewindowsclub_com-medrectangle-1","Deals":[d[17],d[18],d[19],d[20],d[7],d[8],d[9],d[10],d[11],d[12],d[13],d[14]]},{"SlotName":"/1254144/thewindowsclub_com-banner-2","Deals":[d[17],d[18],d[19],d[20],d[7],d[8],d[9],d[10],d[11],d[12],d[13],d[14],d[15],d[16]]},{"SlotName":"/1254144/thewindowsclub_com-box-3","Deals":[d[17],d[18],d[19],d[20],d[21],d[7],d[8],d[9],d[10],d[11],d[12],d[13],d[14],d[15],d[16]]},{"SlotName":"/1254144/thewindowsclub_com-medrectangle-4","Deals":[d[17],d[18],d[19],d[20],d[21],d[7],d[8],d[9],d[10],d[11],d[12],d[13],d[14],d[15],d[16]]}]}();
</script>
<script type='text/javascript'>_ebcids=[138231308856,138231308940,138231308949,138231387842,138231421744,138231421759,138231421774,138231421783,138231421789,138231421792,138242067587,138242067590,138242067602,138242067605,138242067608,138242067614,138242229406,138242229415,138242229421,138242229430];</script>
<script data-ezscrex="false" data-cfasync="false" data-pagespeed-no-defer type='text/javascript'>ezobv=7;</script><script data-ezscrex="false" data-cfasync="false" data-pagespeed-no-defer type='text/javascript'>function ez_isclean(data){if(typeof data==='undefined'){data=document.URL;}
var re=/(([^<>()[\]\\.,;:\s@\"]+(\.[^<>()[\]\\.,;:\s@\"]+)*)|(\".+\"))(@|%2540|%40)((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))/;var isClean=!re.test(data);return isClean;}
var ez_queue=new Array();function sort_queue(a,b)
{if(a.priority<b.priority)return-1;else if(a.priority==b.priority)return 0;else return 1;}
function execute_ez_queue()
{ez_queue.sort(sort_queue);for(var i in ez_queue)
{if(typeof ez_queue[i].method!="undefined")
{try{ez_queue[i].method.call(null);}
catch(err){}}}}
window.ez_ad_units=new Array();window.ezslots=new Array();window.ezsrqt={};function ez_write_tag(d){if(ez_isclean()&&d instanceof Array){if(typeof ezstandalone!=='undefined'&&typeof ezstandalone.selectedPlaceholders!=='undefined'&&ezstandalone.selectedPlaceholders[d[3]]===true){return "1+1";}
ez_ad_units[ez_ad_units.length]=d;var dve="";if(typeof d[5]!='undefined'&&d[5]>0){dve='_'+d[5];}
var ezcmd="googletag.cmd.push(function() {var divid = 'div-gpt-ad-"+d[1]+"-"+d[4]+""+dve+"';if(typeof ezlrarn == 'function'){ezlrarn(divid);}googletag.display(divid);var to = 0;if("+d[2]+".getTargeting('ga')[0] == '0'){to = 500;console.log('"+d[2]+" - no google');}if(window.ezDisableInitialLoad==true || googletag.pubads().isInitialLoadDisabled()){setTimeout(function(){googletag.pubads().refresh(["+d[2]+"])},to);}});";return ezcmd;}
return "1+1";}
function in_array(needle,haystack){var length=haystack.length;for(var i=0;i<length;i++){if(haystack[i]==needle)return true;}
return false;}
var ezrpos=new Array();var ez_current_interval;var ez_current_load=0;</script><script data-cfasync="false" type="text/javascript" data-pagespeed-no-defer src="//go.ezodn.com/hb/dall.js?b=amx,appnexus,brightcom,conversant,criteo,districtm,districtmDMX,gumgum,ix,lockerdome,luponmedia,oftmedia,oneVideo,onemobile,onetag,openx,pubmatic,pulsepoint,rhythmone,rubicon,sovrn,spotx,triplelift,undertone,unruly&cb=192-3-11" async></script><script data-ezscrex="false" data-cfasync="false" type="text/javascript" data-pagespeed-no-defer>var epbjs=epbjs||{};epbjs.que=epbjs.que||[];epbjs.bidderTimeout=2000;epbjs.useAdj=true;epbjs.SS={"amx":11290,"appnexus":10087,"brightcom":11294,"conversant":10033,"criteo":10050,"districtm":10035,"districtmDMX":10090,"gumgum":10079,"ix":10082,"lockerdome":10085,"luponmedia":11300,"oftmedia":10081,"oneVideo":11299,"onemobile":11293,"onetag":11291,"openx":10015,"pubmatic":10061,"pulsepoint":11301,"rhythmone":11298,"rubicon":10063,"sovrn":10017,"spotx":11304,"triplelift":11296,"undertone":11292,"unruly":10097};epbjs.bidders=['amx,appnexus,brightcom,conversant,criteo,districtm,districtmDMX,gumgum,ix,lockerdome,luponmedia,oftmedia,oneVideo,onemobile,onetag,openx,pubmatic,pulsepoint,rhythmone,rubicon,sovrn,spotx,triplelift,undertone,unruly'];epbjs.que.push(function(){epbjs.aliasBidder('appnexus', 'conversant');epbjs.aliasBidder('appnexus', 'districtm');epbjs.aliasBidder('appnexus', 'oftmedia');});epbjs.bidderSettings={'districtmDMX': { bidCpmAdjustment: function(bidCpm) { var adj1 = bidCpm * 1.000000; var adj2 = adj1 * 1.000000; return adj2; }},'conversant': { bidCpmAdjustment: function(bidCpm) { var adj1 = bidCpm * 0.800000; var adj2 = adj1 * 1.000000; return adj2; }},'districtm': { bidCpmAdjustment: function(bidCpm) { var adj1 = bidCpm * 0.890000; var adj2 = adj1 * 1.000000; return adj2; }},'lockerdome': { bidCpmAdjustment: function(bidCpm) { var adj1 = bidCpm * 1.000000; var adj2 = adj1 * 1.000000; return adj2; }},'sovrn': { bidCpmAdjustment: function(bidCpm) { var adj1 = bidCpm * 1.000000; var adj2 = adj1 * 1.000000; return adj2; }},'openx': { bidCpmAdjustment: function(bidCpm) { var adj1 = bidCpm * 1.000000; var adj2 = adj1 * 1.000000; return adj2; }},'oftmedia': { bidCpmAdjustment: function(bidCpm) { var adj1 = bidCpm * 0.850000; var adj2 = adj1 * 1.000000; return adj2; }},'ix': { bidCpmAdjustment: function(bidCpm) { var adj1 = bidCpm * 0.950000; var adj2 = adj1 * 1.000000; return adj2; }},'gumgum': { bidCpmAdjustment: function(bidCpm) { var adj1 = bidCpm * 1.000000; var adj2 = adj1 * 1.000000; return adj2; }},'onemobile': { bidCpmAdjustment: function(bidCpm) { var adj1 = bidCpm * 0.900000; var adj2 = adj1 * 1.000000; return adj2; }},'criteo': { bidCpmAdjustment: function(bidCpm) { var adj1 = bidCpm * 0.900000; var adj2 = adj1 * 1.000000; return adj2; }},'pubmatic': { bidCpmAdjustment: function(bidCpm) { var adj1 = bidCpm * 1.000000; var adj2 = adj1 * 1.000000; return adj2; }},'amx': { bidCpmAdjustment: function(bidCpm) { var adj1 = bidCpm * 0.800000; var adj2 = adj1 * 1.000000; return adj2; }},'onetag': { bidCpmAdjustment: function(bidCpm) { var adj1 = bidCpm * 1.000000; var adj2 = adj1 * 1.000000; return adj2; }},'undertone': { bidCpmAdjustment: function(bidCpm) { var adj1 = bidCpm * 1.000000; var adj2 = adj1 * 1.000000; return adj2; }},'brightcom': { bidCpmAdjustment: function(bidCpm) { var adj1 = bidCpm * 1.000000; var adj2 = adj1 * 1.000000; return adj2; }},'rubicon': { bidCpmAdjustment: function(bidCpm) { var adj1 = bidCpm * 1.000000; var adj2 = adj1 * 1.000000; return adj2; }},'triplelift': { bidCpmAdjustment: function(bidCpm) { var adj1 = bidCpm * 1.000000; var adj2 = adj1 * 1.000000; return adj2; }},'unruly': { bidCpmAdjustment: function(bidCpm) { var adj1 = bidCpm * 0.490000; var adj2 = adj1 * 1.000000; return adj2; }},'appnexus': { bidCpmAdjustment: function(bidCpm) { var adj1 = bidCpm * 0.950000; var adj2 = adj1 * 1.000000; return adj2; }},'rhythmone': { bidCpmAdjustment: function(bidCpm) { var adj1 = bidCpm * 1.000000; var adj2 = adj1 * 1.000000; return adj2; }},'oneVideo': { bidCpmAdjustment: function(bidCpm) { var adj1 = bidCpm * 0.260000; var adj2 = adj1 * 1.000000; return adj2; }},'pulsepoint': { bidCpmAdjustment: function(bidCpm) { var adj1 = bidCpm * 1.000000; var adj2 = adj1 * 1.000000; return adj2; }},'spotx': { bidCpmAdjustment: function(bidCpm) { var adj1 = bidCpm * 1.000000; var adj2 = adj1 * 1.000000; return adj2; }},};epbjs.gadj=1.000000;var __enableAnalytics=false;
__ez.queue.addFile('/detroitchicago/houston.js', '/detroitchicago/houston.js?gcb=3&cb=36', false, [], true, false, true, false);__ez.queue.addFunc("epbjsRequestAdUnits", "epbjsRequestAdUnits", [[{code: 'div-gpt-ad-thewindowsclub_com-box-3-0', mediaTypes: {video: { context:'outstream', playerSize:[[300, 250]] }}, bids: [{bidder: 'unruly', params:{ siteId: '217328', targetingUUID: '217328' }},{bidder: 'oneVideo', params: { pubId: 'EzoicInc', video: {playerWidth: 300, playerHeight: 250, mimes: ['video/mp4', 'application/javascript'], protocols: [2], api: [1,2], placement: 2} }},{bidder: 'spotx', params: { channel_id: '309672', ad_unit: 'outstream', outstream_options: {slot: 'div-gpt-ad-thewindowsclub_com-box-3-0'} }}] },{code: 'div-gpt-ad-thewindowsclub_com-box-3-0', mediaTypes: {banner: { sizes:[[300,250]] }}, bids: [{bidder: 'districtm', params: { placementId: '20459503' }},{bidder: 'districtmDMX', params: { dmxid: '568187', memberid: '100604'}},{bidder: 'conversant', params: { site_id: '121154', secure: 1 }},{bidder: 'sovrn', params: { tagid: '593601'}},{bidder: 'openx',params: { delDomain: 'ezoic-d.openx.net', unit: '538151781' }},{bidder: 'oftmedia', params:{ placementId: '19594014', video: {skippable: true, playback_method: ['auto_play_sound_off']}}},{bidder: 'ix', params: { siteId: '305138', size: [300,250] }},{bidder: 'gumgum', params:{ inSlot: '20833' }},{bidder: 'onemobile', params: { pos: '8a9691b20174742046e22112567001b1', dcn: '8a9691b20174742046e2210bface012a' }},{bidder: 'criteo', params: { networkId: '7987' }},{bidder: 'pubmatic', params:{ publisherId: '156983', adSlot: 'e_under_page_title_300x250' }},{bidder: 'amx', params: { tagId: 'ZXpvaWMuY29t' }},{bidder: 'onetag', params: { pubId: '62499636face9dc' }},{bidder: 'undertone', params: { publisherId: '4009', placementId: '4009001' }},{bidder: 'brightcom', params: { publisherId: '20305' }},{bidder: 'rubicon', params:{ accountId: '21150', siteId: '273012', zoneId: '1361802' }},{bidder: 'triplelift', params: { inventoryCode: 'Ezoic_RON_UnderPageTitle'}},{bidder: 'rhythmone', params: { placementId: '215626' }},{bidder: 'luponmedia', params: { keyId: 'thewindowsclubcom300x250', siteId: 1177 }},{bidder: 'pulsepoint', params: { cf: '300x250', cp: '562406', ct: '719185' }}] },{code: 'div-gpt-ad-thewindowsclub_com-medrectangle-3-0', mediaTypes: {video: { context:'outstream', playerSize:[[580, 400]] }}, bids: [{bidder: 'unruly', params:{ siteId: '217328', targetingUUID: '217328' }}] },{code: 'div-gpt-ad-thewindowsclub_com-medrectangle-3-0', mediaTypes: {banner: { sizes:[[580,400]] }}, bids: [{bidder: 'ix', params: { siteId: '305142', size: [580,400] }},{bidder: 'pubmatic', params:{ publisherId: '156983', adSlot: 'e_under_first_paragraph_580x400' }},{bidder: 'amx', params: { tagId: 'ZXpvaWMuY29t' }},{bidder: 'triplelift', params: { inventoryCode: 'Ezoic_RON_UnderFirstParagraph'}},{bidder: 'rhythmone', params: { placementId: '215626' }}] },{code: 'div-gpt-ad-thewindowsclub_com-banner-2-0', mediaTypes: {video: { context:'outstream', playerSize:[[300, 600]] }}, bids: [{bidder: 'unruly', params:{ siteId: '217328', targetingUUID: '217328' }},{bidder: 'oneVideo', params: { pubId: 'EzoicInc', video: {playerWidth: 300, playerHeight: 600, mimes: ['video/mp4', 'application/javascript'], protocols: [2], api: [1,2], placement: 2} }},{bidder: 'spotx', params: { channel_id: '309672', ad_unit: 'outstream', outstream_options: {slot: 'div-gpt-ad-thewindowsclub_com-banner-2-0'} }}] },{code: 'div-gpt-ad-thewindowsclub_com-banner-2-0', mediaTypes: {banner: { sizes:[[300,600],[160,600]] }}, bids: [{bidder: 'districtmDMX', params: { dmxid: '568187', memberid: '100604'}},{bidder: 'conversant', params: { site_id: '121154', secure: 1 }},{bidder: 'districtm', params: { placementId: '20459503' }},{bidder: 'sovrn', params: { tagid: '593681'}},{bidder: 'openx',params: { delDomain: 'ezoic-d.openx.net', unit: '538151779' }},{bidder: 'oftmedia', params:{ placementId: '19594057', video: {skippable: true, playback_method: ['auto_play_sound_off']}}},{bidder: 'ix', params: { siteId: '305145', size: [300,600] }},{bidder: 'gumgum', params:{ inSlot: '20866' }},{bidder: 'onemobile', params: { dcn: '8a9691b20174742046e2210bface012a', pos: '8a9691b20174742046e221125ff301b4' }},{bidder: 'criteo', params: { networkId: '7987' }},{bidder: 'pubmatic', params:{ publisherId: '156983', adSlot: 'e_sidebar_floating_1_300x600' }},{bidder: 'amx', params: { tagId: 'ZXpvaWMuY29t' }},{bidder: 'onetag', params: { pubId: '62499636face9dc' }},{bidder: 'brightcom', params: { publisherId: '20305' }},{bidder: 'rubicon', params:{ accountId: '21150', siteId: '273012', zoneId: '1361816' }},{bidder: 'rhythmone', params: { placementId: '215626' }},{bidder: 'luponmedia', params: { keyId: 'thewindowsclubcom300x600', siteId: 1177 }},{bidder: 'pulsepoint', params: { cf: '300x600', cp: '562406', ct: '719189' }}] },{code: 'div-gpt-ad-thewindowsclub_com-box-1-0', mediaTypes: {video: { context:'outstream', playerSize:[[336, 280]] }}, bids: [{bidder: 'unruly', params:{ siteId: '217328', targetingUUID: '217328' }},{bidder: 'oneVideo', params: { pubId: 'EzoicInc', video: {playerWidth: 336, playerHeight: 280, mimes: ['video/mp4', 'application/javascript'], protocols: [2], api: [1,2], placement: 2} }},{bidder: 'spotx', params: { channel_id: '309672', ad_unit: 'outstream', outstream_options: {slot: 'div-gpt-ad-thewindowsclub_com-box-1-0'} }}] ,sizeMapping: [
			{
				minWidth: 300,
				sizes: [[336,280]]
			},
			{
				minWidth: 0,
				sizes: [[300,250],[250,250]]
			}]},{code: 'div-gpt-ad-thewindowsclub_com-box-1-0', mediaTypes: {banner: { sizes:[[336,280],[300,250],[250,250]] }}, bids: [{bidder: 'districtmDMX', params: { dmxid: '568187', memberid: '100604'}},{bidder: 'conversant', params: { site_id: '121154', secure: 1 }},{bidder: 'districtm', params: { placementId: '20459503' }},{bidder: 'sovrn', params: { tagid: '593577'}},{bidder: 'openx',params: { delDomain: 'ezoic-d.openx.net', unit: '538151781' }},{bidder: 'oftmedia', params:{ placementId: '19593629', video: {skippable: true, playback_method: ['auto_play_sound_off']}}},{bidder: 'ix', params: { siteId: '305136', size: [336,280] }},{bidder: 'gumgum', params:{ inSlot: '20829' }},{bidder: 'onemobile', params: { dcn: '8a9691b20174742046e2210bface012a', pos: '8a9691b20174742046e22111a9ab0161' }},{bidder: 'criteo', params: { networkId: '7987' }},{bidder: 'pubmatic', params:{ publisherId: '156983', adSlot: 'e_sidebar_336x280' }},{bidder: 'amx', params: { tagId: 'ZXpvaWMuY29t' }},{bidder: 'onetag', params: { pubId: '62499636face9dc' }},{bidder: 'undertone', params: { publisherId: '4009', placementId: '4009001' }},{bidder: 'brightcom', params: { publisherId: '20305' }},{bidder: 'rubicon', params:{ accountId: '21150', siteId: '273012', zoneId: '1361798' }},{bidder: 'triplelift', params: { inventoryCode: 'Ezoic_RON_Sidebar'}},{bidder: 'rhythmone', params: { placementId: '215626' }},{bidder: 'luponmedia', params: { keyId: 'thewindowsclubcom300x250', siteId: 1177 }},{bidder: 'pulsepoint', params: { cf: '336x280', cp: '562406', ct: '719186' }}] ,sizeMapping: [
			{
				minWidth: 300,
				sizes: [[336,280]]
			},
			{
				minWidth: 0,
				sizes: [[300,250],[250,250]]
			}]},{code: 'div-gpt-ad-thewindowsclub_com-large-mobile-banner-1-0', mediaTypes: {video: { context:'outstream', playerSize:[[580, 400]] }}, bids: [{bidder: 'unruly', params:{ siteId: '217328', targetingUUID: '217328' }},{bidder: 'oneVideo', params: { pubId: 'EzoicInc', video: {playerWidth: 580, playerHeight: 400, mimes: ['video/mp4', 'application/javascript'], protocols: [2], api: [1,2], placement: 2} }},{bidder: 'spotx', params: { channel_id: '309672', ad_unit: 'outstream', outstream_options: {slot: 'div-gpt-ad-thewindowsclub_com-large-mobile-banner-1-0'} }}] },{code: 'div-gpt-ad-thewindowsclub_com-large-mobile-banner-1-0', mediaTypes: {banner: { sizes:[[336,280],[300,250],[580,400]] }}, bids: [{bidder: 'conversant', params: { site_id: '121154', secure: 1 }},{bidder: 'districtm', params: { placementId: '20459503' }},{bidder: 'districtmDMX', params: { dmxid: '568187', memberid: '100604'}},{bidder: 'sovrn', params: { tagid: '794927'}},{bidder: 'openx',params: { delDomain: 'ezoic-d.openx.net', unit: '538151781' }},{bidder: 'gumgum', params:{ inSlot: '16886' }},{bidder: 'onemobile', params: { dcn: '8a9691b20174742046e2210bface012a', pos: '8a9691b20174742046e2211258fd01b2' }},{bidder: 'criteo', params: { networkId: '7987' }},{bidder: 'pubmatic', params:{ publisherId: '156983', adSlot: 'In-Content_300x250_BTF' }},{bidder: 'amx', params: { tagId: 'ZXpvaWMuY29t' }},{bidder: 'onetag', params: { pubId: '62499636face9dc' }},{bidder: 'undertone', params: { publisherId: '4009', placementId: '4009001' }},{bidder: 'brightcom', params: { publisherId: '20305' }},{bidder: 'rubicon', params:{ accountId: '21150', siteId: '351284', zoneId: '1868548' }},{bidder: 'rhythmone', params: { placementId: '215626' }},{bidder: 'luponmedia', params: { keyId: 'thewindowsclubcom300x250', siteId: 1177 }},{bidder: 'pulsepoint', params: { cf: '336x280', cp: '562406', ct: '719186' }}] },{code: 'div-gpt-ad-thewindowsclub_com-medrectangle-1-0', mediaTypes: {video: { context:'outstream', playerSize:[[728, 90]] }}, bids: [{bidder: 'unruly', params:{ siteId: '217328', targetingUUID: '217328' }},{bidder: 'oneVideo', params: { pubId: 'EzoicInc', video: {playerWidth: 728, playerHeight: 90, mimes: ['video/mp4', 'application/javascript'], protocols: [2], api: [1,2], placement: 2} }},{bidder: 'spotx', params: { channel_id: '309672', ad_unit: 'outstream', outstream_options: {slot: 'div-gpt-ad-thewindowsclub_com-medrectangle-1-0'} }}] },{code: 'div-gpt-ad-thewindowsclub_com-medrectangle-1-0', mediaTypes: {banner: { sizes:[[728,90]] }}, bids: [{bidder: 'districtmDMX', params: { dmxid: '568187', memberid: '100604'}},{bidder: 'conversant', params: { site_id: '121154', secure: 1 }},{bidder: 'districtm', params: { placementId: '20459503' }},{bidder: 'sovrn', params: { tagid: '593624'}},{bidder: 'openx',params: { delDomain: 'ezoic-d.openx.net', unit: '538151782' }},{bidder: 'oftmedia', params:{ placementId: '19594037', video: {skippable: true, playback_method: ['auto_play_sound_off']}}},{bidder: 'ix', params: { siteId: '305140', size: [728,90] }},{bidder: 'gumgum', params:{ inSlot: '20889' }},{bidder: 'onemobile', params: { dcn: '8a9691b20174742046e2210bface012a', pos: '8a9691b20174742046e22111c8ee016f' }},{bidder: 'criteo', params: { networkId: '7987' }},{bidder: 'pubmatic', params:{ publisherId: '156983', adSlot: 'e_bottom_of_page_728x90' }},{bidder: 'amx', params: { tagId: 'ZXpvaWMuY29t' }},{bidder: 'onetag', params: { pubId: '62499636face9dc' }},{bidder: 'undertone', params: { placementId: '4009004', publisherId: '4009' }},{bidder: 'brightcom', params: { publisherId: '20305' }},{bidder: 'rubicon', params:{ accountId: '21150', siteId: '273012', zoneId: '1361806' }},{bidder: 'triplelift', params: { inventoryCode: 'Ezoic_RON_BottomOfPage'}},{bidder: 'rhythmone', params: { placementId: '215626' }},{bidder: 'luponmedia', params: { keyId: 'thewindowsclubcom728x90', siteId: 1177 }},{bidder: 'pulsepoint', params: { cf: '728x90', cp: '562406', ct: '719177' }}] },{code: 'div-gpt-ad-thewindowsclub_com-box-2-0', mediaTypes: {video: { context:'outstream', playerSize:[[728, 90]] }}, bids: [{bidder: 'unruly', params:{ siteId: '217328', targetingUUID: '217328' }},{bidder: 'oneVideo', params: { pubId: 'EzoicInc', video: {playerWidth: 728, playerHeight: 90, mimes: ['video/mp4', 'application/javascript'], protocols: [2], api: [1,2], placement: 2} }},{bidder: 'spotx', params: { channel_id: '309672', ad_unit: 'outstream', outstream_options: {slot: 'div-gpt-ad-thewindowsclub_com-box-2-0'} }}] },{code: 'div-gpt-ad-thewindowsclub_com-box-2-0', mediaTypes: {banner: { sizes:[[728,90]] }}, bids: [{bidder: 'districtmDMX', params: { dmxid: '568187', memberid: '100604'}},{bidder: 'conversant', params: { site_id: '121154', secure: 1 }},{bidder: 'districtm', params: { placementId: '20459503' }},{bidder: 'sovrn', params: { tagid: '593590'}},{bidder: 'openx',params: { delDomain: 'ezoic-d.openx.net', unit: '538151782' }},{bidder: 'oftmedia', params:{ placementId: '19594005', video: {skippable: true, playback_method: ['auto_play_sound_off']}}},{bidder: 'ix', params: { siteId: '305137', size: [728,90] }},{bidder: 'gumgum', params:{ inSlot: '20886' }},{bidder: 'onemobile', params: { dcn: '8a9691b20174742046e2210bface012a', pos: '8a9691b20174742046e221120e1f0193' }},{bidder: 'criteo', params: { networkId: '7987' }},{bidder: 'pubmatic', params:{ publisherId: '156983', adSlot: 'e_top_of_page_728x90' }},{bidder: 'amx', params: { tagId: 'ZXpvaWMuY29t' }},{bidder: 'onetag', params: { pubId: '62499636face9dc' }},{bidder: 'undertone', params: { publisherId: '4009', placementId: '4009004' }},{bidder: 'brightcom', params: { publisherId: '20305' }},{bidder: 'rubicon', params:{ accountId: '21150', siteId: '273012', zoneId: '1361800' }},{bidder: 'triplelift', params: { inventoryCode: 'Ezoic_RON_TopOfPage'}},{bidder: 'rhythmone', params: { placementId: '215626' }},{bidder: 'luponmedia', params: { siteId: 1177, keyId: 'thewindowsclubcom728x90' }},{bidder: 'pulsepoint', params: { cf: '728x90', cp: '562406', ct: '719177' }}] }]], false, ['/detroitchicago/houston.js'], true, true, true, true);</script><script type='text/javascript' data-ezscrex="false">var ezorbf = []; </script><script data-ezscrex="false" data-cfasync="false" data-pagespeed-no-defer type='text/javascript'>window.isEZABL=false;window.ezmadspc=300;window.ezoViewCheck=false;</script><script data-ezscrex="false" data-cfasync="false" data-pagespeed-no-defer type='text/javascript'>window.ezDisableInitialLoad=false;</script><script data-ezscrex="false" data-cfasync="false" data-pagespeed-no-defer type='text/javascript'>window.googletag=window.googletag||{};googletag.cmd=googletag.cmd||[];</script><script data-ezscrex="false" data-cfasync="false" data-pagespeed-no-defer type='text/javascript'>(function(){var gads=document.createElement('script');gads.async=true;gads.type='text/javascript';var useSSL='https:'==document.location.protocol;gads.src=(useSSL?'https:':'http:')+
'//securepubads.g.doubleclick.net/tag/js/gpt.js';var node=document.getElementsByTagName('script')[0];node.parentNode.insertBefore(gads,node);})();</script><script data-ezscrex="false" data-cfasync="false" data-pagespeed-no-defer type='text/javascript'>window.ezogetbrkey = function(s){ var k = 'br1';var k2 = 'eb_br';if(window.ezogtk == ""){k='br1u';k2='eb_bru';}else if(window.ezogtk != "NT"){k='br1t';k2='eb_brt';} s.setTargeting('br1', s.getTargeting(k));s.setTargeting('eb_br', s.getTargeting(k2));};googletag.cmd.push(function() {if(typeof window.isEZABL == 'undefined' || window.isEZABL != true) {ezslot_0 = googletag.defineSlot('/1254144/thewindowsclub_com-box-3',[300,250],'div-gpt-ad-thewindowsclub_com-box-3-0').addService(googletag.pubads()).setTargeting('iid15','1422233').setTargeting('t','134').setTargeting('d','77472').setTargeting('t1','134').setTargeting('pvc','1').setTargeting('ap','1144').setTargeting('sap','1144').setTargeting('a','|3|').setTargeting('as','revenue').setTargeting('plat','1').setTargeting('bra','mod21-c').setTargeting('ic','1').setTargeting('at','mbf').setTargeting('adr','399').setTargeting('ezosn','0').setTargeting('reft','tf').setTargeting('refs','30').setTargeting('ga','2497208').setTargeting('gala','').setTargeting('rid','99998').setTargeting('pt','2').setTargeting('al','1002').setTargeting('compid','0').setTargeting('tap','thewindowsclub_com-box-3-1422233').setTargeting('eb_br','6240c545bce1855c4e5a6ca430f526b1').setTargeting('eba','1').setTargeting('ebss',[10017,10082,10061,10015,10063,11304]).setTargeting('asau','7552457001').setTargeting('bv','16').setTargeting('bvm','0').setTargeting('bvr','6').setTargeting('shp','3').setCollapseEmptyDiv(false).setTargeting('br1','2400').setTargeting('br2','1200').setTargeting('ezoic','1').setTargeting('nmau','0').setTargeting('mau','0').setTargeting('stl','34,193,28,67,45,122,66,20,71,30,0,31').setTargeting('deal1',[22,23,24,25,26]).setTargeting('ax_ssid','10082');ezrpos[0]="0";ezslot_5 = googletag.defineSlot('/1254144/thewindowsclub_com-large-mobile-banner-1',[580,400],'div-gpt-ad-thewindowsclub_com-large-mobile-banner-1-0').addService(googletag.pubads()).setTargeting('iid15','1433180').setTargeting('t','134').setTargeting('d','77472').setTargeting('t1','134').setTargeting('pvc','1').setTargeting('ap','1105').setTargeting('sap','1105').setTargeting('a','|3|').setTargeting('as','revenue').setTargeting('plat','1').setTargeting('bra','mod21-c').setTargeting('ic','1').setTargeting('at','mbf').setTargeting('adr','399').setTargeting('ezosn','5').setTargeting('reft','tf').setTargeting('refs','30').setTargeting('ga','2497208').setTargeting('gala','').setTargeting('rid','99998').setTargeting('pt','704').setTargeting('al','1704').setTargeting('compid','0').setTargeting('tap','thewindowsclub_com-large-mobile-banner-1-1433180').setTargeting('eb_br','65b2c11be72ed8610e2ac0304f3023a9').setTargeting('eba','1').setTargeting('ebss',[10017,10082,10061,10015,10063,11304]).setTargeting('asau','7552457001').setTargeting('bv','28').setTargeting('bvm','2').setTargeting('bvr','5').setTargeting('shp','1').setCollapseEmptyDiv(false).setTargeting('br1','1900').setTargeting('br2','950').setTargeting('ezoic','1').setTargeting('nmau','0').setTargeting('mau','0').setTargeting('stl','32,168,28,67,45,122,132,0,71,30,0,31').setTargeting('deal1',[21,22,23,24,25,26]).setTargeting('ax_ssid','10082');ezrpos[5]="5";ezslot_7 = googletag.defineSlot('/1254144/thewindowsclub_com-box-2',[728,90],'div-gpt-ad-thewindowsclub_com-box-2-0').addService(googletag.pubads()).setTargeting('iid15','1464234').setTargeting('t','134').setTargeting('d','77472').setTargeting('t1','134').setTargeting('pvc','1').setTargeting('ap','1894').setTargeting('sap','1894').setTargeting('a','|1|').setTargeting('as','revenue').setTargeting('plat','1').setTargeting('bra','mod21-c').setTargeting('ic','1').setTargeting('at','mbf').setTargeting('adr','399').setTargeting('ezosn','7').setTargeting('reft','tf').setTargeting('refs','30').setTargeting('ga','2497208').setTargeting('gala','').setTargeting('rid','99998').setTargeting('pt','1').setTargeting('al','1001').setTargeting('compid','0').setTargeting('tap','thewindowsclub_com-box-2-1464234').setTargeting('eb_br','e41b3739f340bda9dcfb30f79c9db1c9').setTargeting('eba','1').setTargeting('ebss',[10017,10082,10061,10015,10063,11304]).setTargeting('asau','7552457001').setTargeting('bv','28').setTargeting('bvm','2').setTargeting('bvr','5').setTargeting('shp','1').setTargeting('acptad','1').setCollapseEmptyDiv(false).setTargeting('br1','8000').setTargeting('br2','4000').setTargeting('ezoic','1').setTargeting('nmau','0').setTargeting('mau','0').setTargeting('stl','34,193,28,67,45,0,66,20,71,30,187,31').setTargeting('deal1',[27,28,29,30]).setTargeting('ax_ssid','10082');ezrpos[7]="7";ezslot_3 = googletag.defineSlot('/1254144/thewindowsclub_com-box-1',[336,280],'div-gpt-ad-thewindowsclub_com-box-1-0').addService(googletag.pubads()).setTargeting('iid15','1442631').setTargeting('t','134').setTargeting('d','77472').setTargeting('t1','134').setTargeting('pvc','1').setTargeting('ap','1870').setTargeting('sap','1870').setTargeting('a','|5|').setTargeting('as','revenue').setTargeting('plat','1').setTargeting('bra','mod21-c').setTargeting('ic','1').setTargeting('at','mbf').setTargeting('adr','399').setTargeting('ezosn','3').setTargeting('reft','n').setTargeting('refs','30').setTargeting('ga','2497208').setTargeting('gala','').setTargeting('rid','99998').setTargeting('pt','0').setTargeting('al','1000').setTargeting('compid','0').setTargeting('tap','thewindowsclub_com-box-1-1442631').setTargeting('eb_br','a9ec56005762ef40746ec1b6d554f472').setTargeting('eba','1').setTargeting('ebss',[10017,10082,10061,10015,10063,11304]).setTargeting('asau','7552457001').setTargeting('bv','14').setTargeting('bvm','0').setTargeting('bvr','4').setTargeting('shp','3').setTargeting('acptad','1').setCollapseEmptyDiv(false).setTargeting('br1','2800').setTargeting('br2','1400').setTargeting('ezoic','1').setTargeting('nmau','0').setTargeting('mau','0').setTargeting('stl','77,0,28,4,45,122,196,20,71,30,0,31').setTargeting('deal1',[23,24,25,26]).setTargeting('ax_ssid','10082').defineSizeMapping(googletag.sizeMapping().addSize([300,0], [336,280]).addSize([0,0], [300,250]).addSize([0,0], [250,250]).build());ezrpos[3]="3";ezslot_4 = googletag.defineSlot('/1254144/thewindowsclub_com-medrectangle-4',[300,250],'div-gpt-ad-thewindowsclub_com-medrectangle-4-0').addService(googletag.pubads()).setTargeting('iid15','1487178').setTargeting('t','134').setTargeting('d','77472').setTargeting('t1','134').setTargeting('pvc','1').setTargeting('ap','1600').setTargeting('sap','1600').setTargeting('a','|1|').setTargeting('as','revenue').setTargeting('plat','1').setTargeting('bra','mod21-c').setTargeting('ic','1').setTargeting('at','mbf').setTargeting('adr','399').setTargeting('ezosn','4').setTargeting('reft','tf').setTargeting('refs','30').setTargeting('ga','2497208').setTargeting('gala','').setTargeting('rid','99998').setTargeting('pt','22').setTargeting('al','1022').setTargeting('compid','1').setTargeting('tap','thewindowsclub_com-medrectangle-4-1487178').setTargeting('eb_br','b2ac58e6c0c84fc65f344f47dd85768b').setTargeting('eba','1').setTargeting('ebss',[10017,10082,10061,10015,10063,11304]).setTargeting('asau','7552457001').setTargeting('bv','3').setTargeting('bvm','0').setTargeting('bvr','8').setTargeting('shp','3').setCollapseEmptyDiv(false).setTargeting('br1','2100').setTargeting('br2','1000').setTargeting('ezoic','1').setTargeting('nmau','0').setTargeting('mau','0').setTargeting('stl','34,152,120,4,51,0,88,116,71,30,0,31').setTargeting('deal1',[22,23,24,25,26]).setTargeting('ax_ssid','10082');ezrpos[4]="4";ezslot_1 = googletag.defineSlot('/1254144/thewindowsclub_com-medrectangle-3',[580,400],'div-gpt-ad-thewindowsclub_com-medrectangle-3-0').addService(googletag.pubads()).setTargeting('iid15','1430782').setTargeting('t','134').setTargeting('d','77472').setTargeting('t1','134').setTargeting('pvc','1').setTargeting('ap','1153').setTargeting('sap','1153').setTargeting('a','|5|').setTargeting('as','revenue').setTargeting('plat','1').setTargeting('bra','mod21-c').setTargeting('ic','1').setTargeting('at','mbf').setTargeting('adr','399').setTargeting('ezosn','1').setTargeting('reft','tf').setTargeting('refs','30').setTargeting('ga','2497208').setTargeting('gala','').setTargeting('rid','99998').setTargeting('pt','21').setTargeting('al','1021').setTargeting('compid','0').setTargeting('tap','thewindowsclub_com-medrectangle-3-1430782').setTargeting('eb_br','a2de9c8773c426848d7815dff1d2d44f').setTargeting('eba','1').setTargeting('ebss',[10017,10082,10061,10015,10063,11304]).setTargeting('asau','7552457001').setTargeting('bv','28').setTargeting('bvm','2').setTargeting('bvr','5').setTargeting('shp','1').setCollapseEmptyDiv(false).setTargeting('br1','4400').setTargeting('br2','2200').setTargeting('ezoic','1').setTargeting('nmau','0').setTargeting('mau','0').setTargeting('stl','36,168,28,4,45,122,66,1,71,30,0,31').setTargeting('deal1',[25,26]).setTargeting('ax_ssid','10082');ezrpos[1]="1";ezslot_6 = googletag.defineSlot('/1254144/thewindowsclub_com-medrectangle-1',[728,90],'div-gpt-ad-thewindowsclub_com-medrectangle-1-0').addService(googletag.pubads()).setTargeting('iid15','1471876').setTargeting('t','134').setTargeting('d','77472').setTargeting('t1','134').setTargeting('pvc','1').setTargeting('ap','1121').setTargeting('sap','1121').setTargeting('a','|2|').setTargeting('as','revenue').setTargeting('plat','1').setTargeting('bra','mod21-c').setTargeting('ic','1').setTargeting('at','mbf').setTargeting('adr','399').setTargeting('ezosn','6').setTargeting('reft','tf').setTargeting('refs','30').setTargeting('ga','2497208').setTargeting('gala','').setTargeting('rid','99998').setTargeting('pt','4').setTargeting('al','1004').setTargeting('compid','0').setTargeting('tap','thewindowsclub_com-medrectangle-1-1471876').setTargeting('eb_br','dc3573d5dc41abdf97751be02f53537f').setTargeting('eba','1').setTargeting('ebss',[10017,10082,10061,10015,10063,11304]).setTargeting('asau','7552457001').setTargeting('bv','3').setTargeting('bvm','0').setTargeting('bvr','8').setTargeting('shp','1').setTargeting('acptad','1').setCollapseEmptyDiv(false).setTargeting('br1','800').setTargeting('br2','400').setTargeting('ezoic','1').setTargeting('nmau','0').setTargeting('mau','0').setTargeting('stl','34,168,28,67,45,0,66,0,71,30,0,31').setTargeting('deal1',[21,22,23,24,25,26,15,16]).setTargeting('ax_ssid','10082');ezrpos[6]="6";ezslot_2 = googletag.defineSlot('/1254144/thewindowsclub_com-banner-2',[300,600],'div-gpt-ad-thewindowsclub_com-banner-2-0').addService(googletag.pubads()).setTargeting('iid15','1495879').setTargeting('t','134').setTargeting('d','77472').setTargeting('t1','134').setTargeting('pvc','1').setTargeting('ap','1104').setTargeting('sap','1104').setTargeting('a','|5|').setTargeting('as','revenue').setTargeting('plat','1').setTargeting('bra','mod21-c').setTargeting('ic','1').setTargeting('at','mbf').setTargeting('adr','399').setTargeting('ezosn','2').setTargeting('reft','tf').setTargeting('refs','30').setTargeting('ga','2497208').setTargeting('gala','').setTargeting('rid','99998').setTargeting('pt','31').setTargeting('al','1031').setTargeting('compid','0').setTargeting('tap','thewindowsclub_com-banner-2-1495879').setTargeting('eb_br','d81e229576f8cb8a43ff5c6a8e596727').setTargeting('eba','1').setTargeting('ebss',[10017,10082,10061,10015,10063,11304]).setTargeting('asau','7552457001').setTargeting('bv','19').setTargeting('bvm','0').setTargeting('bvr','9').setTargeting('shp','2').setCollapseEmptyDiv(false).setTargeting('br1','1500').setTargeting('br2','750').setTargeting('ezoic','1').setTargeting('nmau','0').setTargeting('mau','0').setTargeting('stl','83,13,120,67,51,0,66,20,71,209,0,31').setTargeting('deal1',[21,22,23,24,25,26]).setTargeting('ax_ssid','10082');ezrpos[2]="2";}else{window.ezHideLocations=[];window.ezHideLocations.push('div-gpt-ad-thewindowsclub_com-box-3-0');window.ezHideLocations.push('div-gpt-ad-thewindowsclub_com-large-mobile-banner-1-0');ezslot_7 = googletag.defineSlot('/1254144/thewindowsclub_com-box-2',[728,90],'div-gpt-ad-thewindowsclub_com-box-2-0').addService(googletag.pubads()).setTargeting('iid15','1464234').setTargeting('t','134').setTargeting('d','77472').setTargeting('t1','134').setTargeting('pvc','1').setTargeting('ap','1894').setTargeting('sap','1894').setTargeting('a','|1|').setTargeting('as','revenue').setTargeting('plat','1').setTargeting('bra','mod21-c').setTargeting('ic','1').setTargeting('at','mbf').setTargeting('adr','399').setTargeting('ezosn','7').setTargeting('reft','tf').setTargeting('refs','30').setTargeting('ga','2497208').setTargeting('gala','').setTargeting('rid','99998').setTargeting('pt','1').setTargeting('al','1001').setTargeting('compid','0').setTargeting('tap','thewindowsclub_com-box-2-1464234').setTargeting('eb_br','e41b3739f340bda9dcfb30f79c9db1c9').setTargeting('eba','1').setTargeting('ebss',[10017,10082,10061,10015,10063,11304]).setTargeting('asau','7552457001').setTargeting('bv','28').setTargeting('bvm','2').setTargeting('bvr','5').setTargeting('shp','1').setTargeting('acptad','1').setCollapseEmptyDiv(false).setTargeting('br1','8000').setTargeting('br2','4000').setTargeting('ezoic','1').setTargeting('nmau','0').setTargeting('mau','0').setTargeting('stl','34,193,28,67,45,0,66,20,71,30,187,31').setTargeting('deal1',[27,28,29,30]).setTargeting('ax_ssid','10082');ezrpos[7]="7";ezslot_3 = googletag.defineSlot('/1254144/thewindowsclub_com-box-1',[336,280],'div-gpt-ad-thewindowsclub_com-box-1-0').addService(googletag.pubads()).setTargeting('iid15','1442631').setTargeting('t','134').setTargeting('d','77472').setTargeting('t1','134').setTargeting('pvc','1').setTargeting('ap','1870').setTargeting('sap','1870').setTargeting('a','|5|').setTargeting('as','revenue').setTargeting('plat','1').setTargeting('bra','mod21-c').setTargeting('ic','1').setTargeting('at','mbf').setTargeting('adr','399').setTargeting('ezosn','3').setTargeting('reft','n').setTargeting('refs','30').setTargeting('ga','2497208').setTargeting('gala','').setTargeting('rid','99998').setTargeting('pt','0').setTargeting('al','1000').setTargeting('compid','0').setTargeting('tap','thewindowsclub_com-box-1-1442631').setTargeting('eb_br','a9ec56005762ef40746ec1b6d554f472').setTargeting('eba','1').setTargeting('ebss',[10017,10082,10061,10015,10063,11304]).setTargeting('asau','7552457001').setTargeting('bv','14').setTargeting('bvm','0').setTargeting('bvr','4').setTargeting('shp','3').setTargeting('acptad','1').setCollapseEmptyDiv(false).setTargeting('br1','2800').setTargeting('br2','1400').setTargeting('ezoic','1').setTargeting('nmau','0').setTargeting('mau','0').setTargeting('stl','77,0,28,4,45,122,196,20,71,30,0,31').setTargeting('deal1',[23,24,25,26]).setTargeting('ax_ssid','10082').defineSizeMapping(googletag.sizeMapping().addSize([300,0], [336,280]).addSize([0,0], [300,250]).addSize([0,0], [250,250]).build());ezrpos[3]="3";window.ezHideLocations.push('div-gpt-ad-thewindowsclub_com-medrectangle-4-0');window.ezHideLocations.push('div-gpt-ad-thewindowsclub_com-medrectangle-3-0');ezslot_6 = googletag.defineSlot('/1254144/thewindowsclub_com-medrectangle-1',[728,90],'div-gpt-ad-thewindowsclub_com-medrectangle-1-0').addService(googletag.pubads()).setTargeting('iid15','1471876').setTargeting('t','134').setTargeting('d','77472').setTargeting('t1','134').setTargeting('pvc','1').setTargeting('ap','1121').setTargeting('sap','1121').setTargeting('a','|2|').setTargeting('as','revenue').setTargeting('plat','1').setTargeting('bra','mod21-c').setTargeting('ic','1').setTargeting('at','mbf').setTargeting('adr','399').setTargeting('ezosn','6').setTargeting('reft','tf').setTargeting('refs','30').setTargeting('ga','2497208').setTargeting('gala','').setTargeting('rid','99998').setTargeting('pt','4').setTargeting('al','1004').setTargeting('compid','0').setTargeting('tap','thewindowsclub_com-medrectangle-1-1471876').setTargeting('eb_br','dc3573d5dc41abdf97751be02f53537f').setTargeting('eba','1').setTargeting('ebss',[10017,10082,10061,10015,10063,11304]).setTargeting('asau','7552457001').setTargeting('bv','3').setTargeting('bvm','0').setTargeting('bvr','8').setTargeting('shp','1').setTargeting('acptad','1').setCollapseEmptyDiv(false).setTargeting('br1','800').setTargeting('br2','400').setTargeting('ezoic','1').setTargeting('nmau','0').setTargeting('mau','0').setTargeting('stl','34,168,28,67,45,0,66,0,71,30,0,31').setTargeting('deal1',[21,22,23,24,25,26,15,16]).setTargeting('ax_ssid','10082');ezrpos[6]="6";window.ezHideLocations.push('div-gpt-ad-thewindowsclub_com-banner-2-0');}googletag.pubads().addEventListener('slotRenderEnded', function(event) { __ez.queue.addFunc("ezbanger", "ezbanger", event, false, ['banger.js'], true, true, false, true); });googletag.pubads().addEventListener('impressionViewable', function(event) { __ez.queue.addFunc("ezvb", "ezvb", event, false, ['banger.js'], true, true, false, true); });googletag.pubads().addEventListener('slotResponseReceived', function(event) { __ez.queue.addFunc("ezsr", "ezsr", event, false, ['banger.js'], true, true, false, true); });googletag.pubads().addEventListener('slotRequested', function(e) { window.ezsrqt[e.slot.getSlotElementId()] = Date.now();});googletag.pubads().enableLazyLoad({fetchMarginPercent: 400, renderMarginPercent: 150, mobileScaling: 2.0});googletag.enableServices();});window.ezoll = false;window.ezoadxnc = '1254144';window.ezorefgsl=function(r){Array.isArray(r)||(r=[r]);for(var e=r.length,o=Array(),a=0;a<e;a++){var t=r[a];t.setTargeting("reqt",Date.now()),void 0!==t.DFPSlot?o.push(t.DFPSlot):o.push(t)}googletag.pubads().refresh(o)};var ezoibfh = Array();ezoibfh[0] = 'zero';ezoibfh[1000000] = 'off';ezoibfh[2800]='a9ec56005762ef40746ec1b6d554f472';
ezoibfh[2100]='b2ac58e6c0c84fc65f344f47dd85768b';
ezoibfh[1200]='736e09a0771285737509ab8954c475a7';
ezoibfh[1000]='c5429b6ddd929d0bc40a832a87789a7c';
ezoibfh[8000]='e41b3739f340bda9dcfb30f79c9db1c9';
ezoibfh[7000]='4552fb4beab2a055aec0d6113a8d9e42';
ezoibfh[3400]='2c0082dd1efc5e4dfdd4f50677fea822';
ezoibfh[2900]='ef3231a19d034bff92faf99318a47a5f';
ezoibfh[260]='57914c3716312cb7e954090f0717ea25';
ezoibfh[120]='58ef7bddb438af5e257c4377f32c243a';
ezoibfh[950]='c410f2a2b0c2123f4b6651cda6c5cf53';
ezoibfh[750]='6ac330e431a70c7d8ce9fb95aee95c72';
ezoibfh[400]='76163170a8636ae5b88417f095893e08';
ezoibfh[280]='c16fac08e79a971524b1c6834f5caad3';
ezoibfh[6000]='49d60519eec4f00cfb2d91dec1e48d41';
ezoibfh[4200]='e9b52ed700c176b9b3f036aa176f3f3e';
ezoibfh[700]='8b07bae800b215e481d05a271b3e723b';
ezoibfh[180]='9ae587f95e95c876b7b76fd4c72a3838';
ezoibfh[1600]='6dbaa2f5e27e83e2fcd15988d9095988';
ezoibfh[50]='3ba982fc4238dd4197b1d51b345478dc';
ezoibfh[6500]='b6ac10cddc8471927cec0144110502e9';
ezoibfh[2500]='78e9436ba8e29037bc31f94589331e0b';
ezoibfh[2300]='a835e008e248a793da87524a4919f755';
ezoibfh[1800]='72c13a89ac876aaffdde39253459460b';
ezoibfh[240]='8de2c8ca79e8623e3cb37120a35ebaa2';
ezoibfh[44]='a928cf2c3ad36f5e9ed2d90f655c1dc9';
ezoibfh[24]='e66c30deca31b19eda212eeca1258584';
ezoibfh[20]='7432360301409ae695ba255f16fbcf06';
ezoibfh[3800]='58e03b675175bbbec8566d319041c5ee';
ezoibfh[1700]='ff69c327c284033fca821ae81630bfa9';
ezoibfh[1500]='d81e229576f8cb8a43ff5c6a8e596727';
ezoibfh[900]='eeb0e32289ff31f9ddef18331038e5e9';
ezoibfh[10]='291d27313eb66c50243129b23df8a579';
ezoibfh[2]='b6c98a8bb15764f1c4ee331dcb724178';
ezoibfh[2400]='6240c545bce1855c4e5a6ca430f526b1';
ezoibfh[160]='3530fcb6bcc13dc3c1712eaef7d92700';
ezoibfh[48]='8fc09e60bfd78aa82afac0405213359a';
ezoibfh[500]='5f2b94bb26a5aa9b1a00e66d30cfd5ec';
ezoibfh[38]='23b5ca1d9de2587e6a4ecfd33d61b709';
ezoibfh[6]='33dd523f8e4dda158f0aa99686dda7f2';
ezoibfh[3600]='81f896ad12450b2f0257b1df6d3f1edc';
ezoibfh[1400]='04b5efc3207e2390972f099a6a3c4757';
ezoibfh[850]='5297de5240aa45da173a0792747e0d26';
ezoibfh[800]='dc3573d5dc41abdf97751be02f53537f';
ezoibfh[14]='ad0061a38dd7c6f7bcb692aee88dfda4';
ezoibfh[1100]='39abb99448d54704c4afa42efe76e15d';
ezoibfh[300]='90c3c48d0172916d27c102ea4aa9d49c';
ezoibfh[60]='c352ba581bd3ffd8cea608cf2d55f519';
ezoibfh[16]='e29f69dd468d31a5514dc9b5587ce757';
ezoibfh[600]='45a351e981f435b4c20fafca8a5d741c';
ezoibfh[220]='43aa1607a0c08c74b14a9039e7b909b4';
ezoibfh[200]='86802a923a1f32517e4c5d3b6d550271';
ezoibfh[34]='a7a863b24978e69c4cdbb5a49be70d5e';
ezoibfh[4400]='a2de9c8773c426848d7815dff1d2d44f';
ezoibfh[3000]='92831edb305b955e915a7cc2288d5df6';
ezoibfh[2700]='401612ca672af30f67eaf5e0989ce385';
ezoibfh[1300]='bfa042bdb1583c959161b7823290dc1f';
ezoibfh[26]='bf9a045b836005b6c23b7b0749249612';
ezoibfh[80]='dfa60cee6e1053fc0c9e607c8047bd28';
ezoibfh[36]='8c5ffefb122f59a66a8b7672d4452af2';
ezoibfh[12]='14e8a85d4c42ff1db8790cbef9e33493';
ezoibfh[4800]='f0459c7057d45e6fbbed62c0762b551e';
ezoibfh[140]='af063c244089b52ec5a0423a258f1f8e';
ezoibfh[100]='a495ce7dbb4cefcd3e0a722048894f41';
ezoibfh[42]='947f1d5169cc7d0f997560e34838fb04';
ezoibfh[550]='26dfa00588543c52511429ade391f561';
ezoibfh[90]='b355e9227b551c119a30a68852723b62';
ezoibfh[18]='8de355ef1cf56b7da61277050d9957b1';
ezoibfh[22]='1e913e99b80640fd5b86a539e5b97c94';
ezoibfh[8]='2e8b8c60843e52e5aaa1e3a52287a2bb';
ezoibfh[7500]='0de5c793b95df3adacbee8e14c308afc';
ezoibfh[4000]='e95a0029a1c0d52e1f82ee010826e7d9';
ezoibfh[2000]='12a3b3570adcf20fd41a00445219acaa';
ezoibfh[46]='fe5b0c99ab7ba15f050582be1301303f';
ezoibfh[5500]='b069a06daabd6e3043166f0e7a2edef4';
ezoibfh[350]='9e0a1ce5b2455cb9b48d5df4c6bf4053';
ezoibfh[30]='54d0fa6d5f6aabe7623cb24faa42a441';
ezoibfh[40]='ee685f77592ce296910ee91457d66ba3';
ezoibfh[4]='9c3e4ee8eae7f1433cb2fe69b1326605';
ezoibfh[5000]='116f73d8738ced0c5546d5313109581e';
ezoibfh[2600]='cc65d2d1fcda72df55233f97cf215dad';
ezoibfh[450]='6e85b37de1b1ffc2593baa5d6e4b02fc';
ezoibfh[70]='527e52c10635ac8136a4c84094ee49a8';
ezoibfh[4600]='d297138284357206d38c781a2291b99a';
ezoibfh[650]='5bac35e1a3b6adc56da706000a645484';
ezoibfh[28]='674294a1b21a1e89fc99c14c9b17be44';
ezoibfh[3200]='41ad5c6ea7dab736638507e437e60604';
ezoibfh[2200]='2620dac3b050a8e36c132f49cccab5a1';
ezoibfh[1900]='65b2c11be72ed8610e2ac0304f3023a9';
ezoibfh[32]='d31e71883d00099e275b6c5878eed023';
var ezaxmns={};var ezaucmns={};ezaxmns["div-gpt-ad-thewindowsclub_com-box-3-0"]=0;ezaucmns["div-gpt-ad-thewindowsclub_com-box-3-0"]=0;ezaxmns["div-gpt-ad-thewindowsclub_com-large-mobile-banner-1-0"]=0;ezaucmns["div-gpt-ad-thewindowsclub_com-large-mobile-banner-1-0"]=0;ezaxmns["div-gpt-ad-thewindowsclub_com-box-2-0"]=0;ezaucmns["div-gpt-ad-thewindowsclub_com-box-2-0"]=0;ezaxmns["div-gpt-ad-thewindowsclub_com-box-1-0"]=0;ezaucmns["div-gpt-ad-thewindowsclub_com-box-1-0"]=0;ezaxmns["div-gpt-ad-thewindowsclub_com-medrectangle-4-0"]=0;ezaucmns["div-gpt-ad-thewindowsclub_com-medrectangle-4-0"]=0;ezaxmns["div-gpt-ad-thewindowsclub_com-medrectangle-3-0"]=0;ezaucmns["div-gpt-ad-thewindowsclub_com-medrectangle-3-0"]=0;ezaxmns["div-gpt-ad-thewindowsclub_com-medrectangle-1-0"]=0;ezaucmns["div-gpt-ad-thewindowsclub_com-medrectangle-1-0"]=0;ezaxmns["div-gpt-ad-thewindowsclub_com-banner-2-0"]=0;ezaucmns["div-gpt-ad-thewindowsclub_com-banner-2-0"]=0;if(typeof window.isEZABL == 'undefined' || window.isEZABL != true) {ezslots.push("ezslot_0");ezslots.push("ezslot_5");ezslots.push("ezslot_7");ezslots.push("ezslot_3");ezslots.push("ezslot_4");ezslots.push("ezslot_1");ezslots.push("ezslot_6");ezslots.push("ezslot_2");}else{ezslots.push("ezslot_7");ezslots.push("ezslot_3");ezslots.push("ezslot_6");}</script>
<script type="text/javascript">(function(){function storageAvailable(type){var storage;try{storage=window[type];var x='__storage_test__';storage.setItem(x,x);storage.removeItem(x);return true;}
catch(e){return e instanceof DOMException&&(e.code===22||e.code===1014||e.name==='QuotaExceededError'||e.name==='NS_ERROR_DOM_QUOTA_REACHED')&&(storage&&storage.length!==0);}}
function remove_ama_config(){if(storageAvailable('localStorage')){localStorage.removeItem("google_ama_config");}}
remove_ama_config()})()</script>
<script type="text/javascript">var ezoicTestActive = true</script>
<script data-ezscrex="false" type="text/javascript" data-cfasync="false">var _ezaq = {"ad_cache_level":2,"ad_count_adjustment":2,"ad_lazyload_version":4,"ad_location_ids":"2,21,31,0,22,704,4,1","ad_transform_level":0,"adx_ad_count":7,"bidder_method":0,"bidder_version":3,"city":"Burnsville","country":"US","days_since_last_visit":0,"display_ad_count":8,"domain_id":77472,"domain_test_group":20200404,"ds_adsize_opt_id":-1,"engaged_time_visit":48,"ezcache_level":2,"ezcache_skip_code":0,"form_factor_id":1,"framework_id":1,"has_bad_image":0,"has_bad_words":0,"iab_category":"","iab_category_0":"596","iab_category_1":"615","iab_category_2":"602","is_from_recommended_pages":false,"is_return_visitor":false,"is_sitespeed":0,"last_page_load":"1614896481574","last_pageview_id":"e3654d48-f6c2-49d3-7510-16e8c3cc7117","lt_cache_level":0,"max_ads":6,"metro_code":613,"optimization_version":0,"page_ad_positions":"1104,1105,1121,1144,1153,1600,1870,1894","page_view_count":1,"page_view_id":"c2eeeada-291f-4952-4ff1-a0e3639cb84d","position_selection_id":39,"postal_code":"55337","pv_event_count":0,"response_size_orig":158111,"response_time_orig":5,"serverid":"35.171.228.123:17862","state":"MN","sub_page_ad_positions":"1104,1105,1121,1144,1153,1600,1870,1894","t_epoch":1614900142,"template_id":134,"time_on_site_visit":57,"url":"https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10","user_id":0,"word_count":620,"worst_bad_word_level":0};var _ezim_d = {"thewindowsclub_com-banner-2":{"adsense_stat_source_id":5,"adx_ad_count":7,"adx_stat_source_id":35,"full_id":"thewindowsclub_com-banner-2/2021-03-04/1495879","height":"600","position_id":1104,"sub_position_id":1104,"width":"300"},"thewindowsclub_com-box-1":{"adsense_stat_source_id":5,"adx_ad_count":7,"adx_stat_source_id":35,"full_id":"thewindowsclub_com-box-1/2021-03-04/1442631","height":"280","position_id":1870,"sub_position_id":1870,"width":"336"},"thewindowsclub_com-box-2":{"adsense_stat_source_id":5,"adx_ad_count":7,"adx_stat_source_id":35,"full_id":"thewindowsclub_com-box-2/2021-03-04/1464234","height":"90","position_id":1894,"sub_position_id":1894,"width":"728"},"thewindowsclub_com-box-3":{"adsense_stat_source_id":5,"adx_ad_count":7,"adx_stat_source_id":35,"full_id":"thewindowsclub_com-box-3/2021-03-04/1422233","height":"250","position_id":1144,"sub_position_id":1144,"width":"300"},"thewindowsclub_com-large-mobile-banner-1":{"adsense_stat_source_id":5,"adx_ad_count":7,"adx_stat_source_id":35,"full_id":"thewindowsclub_com-large-mobile-banner-1/2021-03-04/1433180","height":"400","position_id":1105,"sub_position_id":1105,"width":"580"},"thewindowsclub_com-medrectangle-1":{"adsense_stat_source_id":5,"adx_ad_count":7,"adx_stat_source_id":35,"full_id":"thewindowsclub_com-medrectangle-1/2021-03-04/1471876","height":"90","position_id":1121,"sub_position_id":1121,"width":"728"},"thewindowsclub_com-medrectangle-3":{"adsense_stat_source_id":5,"adx_ad_count":7,"adx_stat_source_id":35,"full_id":"thewindowsclub_com-medrectangle-3/2021-03-04/1430782","height":"400","position_id":1153,"sub_position_id":1153,"width":"580"},"thewindowsclub_com-medrectangle-4":{"adsense_stat_source_id":5,"adx_ad_count":7,"adx_stat_source_id":35,"full_id":"thewindowsclub_com-medrectangle-4/2021-03-04/1487178","height":"250","position_id":1600,"sub_position_id":1600,"width":"300"}};var _ezat = {"domain_id":77472,"form_factor_id":1,"framework_id":1,"pageview_date":"2021-03-04","pageview_id":"c2eeeada-291f-4952-4ff1-a0e3639cb84d","template_id":134,"url":"https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10","visit_uuid":"9895745a-bb0c-43b2-4b2a-0408670806e6"};</script><script data-ezscrex='false' data-pagespeed-no-defer data-cfasync='false' type="text/javascript">__ez.queue.addFile('banger.js', '/porpoiseant/banger.js?cb=192-3&bv=7&v=45&PageSpeed=off', true, [], true, false, false, true);</script>
<script data-ezscrex='false' data-cfasync='false' data-pagespeed-no-defer>__ez.queue.addFile('/detroitchicago/memphis.js', '/detroitchicago/memphis.js?gcb=192-3&cb=5', false, [], true, false, true, false);__ez.queue.addFile('/detroitchicago/minneapolis.js', '/detroitchicago/minneapolis.js?gcb=192-3&cb=3', false, [], true, false, true, false);__ez.queue.addFile('/detroitchicago/rochester.js', '/detroitchicago/rochester.js?gcb=192-3&cb=2', false, [], true, false, true, false);__ez.vep=(function(){var pixels=[],pxURL="/detroitchicago/grapefruit.gif";function AddPixel(vID,pixelData){if(__ez.dot.isDefined(vID)&&__ez.dot.isValid(pixelData)){pixels.push({type:'video',video_impression_id:vID,domain_id:__ez.dot.getDID(),t_epoch:__ez.dot.getEpoch(0),data:__ez.dot.dataToStr(pixelData)});}}
function Fire(){if(typeof document.visibilityState!=='undefined'&&document.visibilityState==="prerender"){return;}
if(__ez.dot.isDefined(pixels)&&pixels.length>0){while(pixels.length>0){var j=5;if(j>pixels.length){j=pixels.length;}
var pushPixels=pixels.splice(0,j);var pixelURL=__ez.dot.getURL(pxURL)+"?orig="+(__ez.template.isOrig===true?1:0)+"&v="+btoa(JSON.stringify(pushPixels));__ez.dot.Fire(pixelURL);}}
pixels=[];}
return{Add:AddPixel,Fire:Fire};})();</script><script data-ezscrex='false' data-cfasync='false' data-pagespeed-no-defer>__ez.pel=(function(){var pixels=[],pxURL="/porpoiseant/army.gif";function AddAndFirePixel(adSlot,pixelData){AddPixel(adSlot,pixelData,0,0,0,0,0);Fire();}
function AddAndFireOrigPixel(adSlot,pixelData){AddPixel(adSlot,pixelData,0,0,0,0,0,true);Fire();}
function GetCurrentPixels(){return pixels;}
function AddPixel(adSlot,pixelData,revenue,est_revenue,bid_floor_filled,bid_floor_prev,stat_source_id,isOrig){if(!__ez.dot.isDefined(adSlot)||__ez.dot.isAnyDefined(adSlot.getSlotElementId,adSlot.ElementId)==false){return;}
var ad_position_id=parseInt(__ez.dot.getTargeting(adSlot,'ap'));var impId=__ez.dot.getSlotIID(adSlot),adUnit=__ez.dot.getAdUnit(adSlot,isOrig);var compId=parseInt(__ez.dot.getTargeting(adSlot,"compid"));var lineItemId=0;var creativeId=0;var ezimData=getEzimData(adSlot);if(typeof ezimData=='object'){if(ezimData.creative_id!==undefined){creativeId=ezimData.creative_id;}
if(ezimData.line_item_id!==undefined){lineItemId=ezimData.line_item_id;}}
if(__ez.dot.isDefined(impId,adUnit)&&__ez.dot.isValid(pixelData)){pixels.push({type:"impression",impression_id:impId,domain_id:__ez.dot.getDID(),unit:adUnit,t_epoch:__ez.dot.getEpoch(0),revenue:revenue,est_revenue:est_revenue,ad_position:ad_position_id,ad_size:"",bid_floor_filled:bid_floor_filled,bid_floor_prev:bid_floor_prev,stat_source_id:stat_source_id,country_code:__ez.dot.getCC(),pageview_id:__ez.dot.getPageviewId(),comp_id:compId,line_item_id:lineItemId,creative_id:creativeId,data:__ez.dot.dataToStr(pixelData),is_orig:isOrig||__ez.template.isOrig,});}}
function AddPixelById(impFullId,pixelData,isOrig){var vals=impFullId.split('/');if(__ez.dot.isDefined(impFullId)&&vals.length===3&&__ez.dot.isValid(pixelData)){var adUnit=vals[0],impId=vals[2];pixels.push({type:"impression",impression_id:impId,domain_id:__ez.dot.getDID(),unit:adUnit,t_epoch:__ez.dot.getEpoch(0),pageview_id:__ez.dot.getPageviewId(),data:__ez.dot.dataToStr(pixelData),is_orig:isOrig||__ez.template.isOrig});}}
function Fire(){if(typeof document.visibilityState!=='undefined'&&document.visibilityState==="prerender")return;if(__ez.dot.isDefined(pixels)&&pixels.length>0){var allPixels=[pixels.filter(function(pixel){return pixel.is_orig}),pixels.filter(function(pixel){return!pixel.is_orig})];allPixels.forEach(function(pixels){while(pixels.length>0){var isOrig=pixels[0].is_orig||false;var j=5;if(j>pixels.length){j=pixels.length;}
var pushPixels=pixels.splice(0,j);var pixelURL=__ez.dot.getURL(pxURL)+"?orig="+(isOrig===true?1:0)+"&sts="+btoa(JSON.stringify(pushPixels));if(typeof window.isAmp!=='undefined'&&isAmp&&typeof window._ezaq!=='undefined'&&_ezaq.hasOwnProperty("domain_id")){pixelURL+="&visit_uuid="+_ezaq['visit_uuid'];}
__ez.dot.Fire(pixelURL);}})}
pixels=[];}
function getEzimData(adSlot){if(typeof _ezim_d=="undefined"){return false}
var adUnitName=__ez.dot.getAdUnitPath(adSlot).split('/').pop();if(typeof _ezim_d==='object'&&_ezim_d.hasOwnProperty(adUnitName)){return _ezim_d[adUnitName];}
for(var ezimKey in _ezim_d){if(ezimKey.split('/').pop()===adUnitName){return _ezim_d[ezimKey];}}
return false;}
return{Add:AddPixel,AddAndFire:AddAndFirePixel,AddAndFireOrig:AddAndFireOrigPixel,AddById:AddPixelById,Fire:Fire,GetPixels:GetCurrentPixels,};})();__ez.queue.addFile('/detroitchicago/raleigh.js', '/detroitchicago/raleigh.js?gcb=192-3&cb=5', false, [], true, false, true, false);__ez.queue.addFile('/detroitchicago/tampa.js', '/detroitchicago/tampa.js?gcb=192-3&cb=3', false, [], true, false, true, false);</script>
	
	<meta name="viewport" content="width=device-width, initial-scale=1"/>
	<link rel="pingback" href="https://www.thewindowsclub.com/xmlrpc.php"/>

	
<!-- Powered by Social Snap v1.1.15 - https://socialsnap.com/ -->
<meta property="og:type" content="article"/>
<meta property="og:title" content="How to run .sh or Shell Script file in Windows 10"/>
<meta property="og:description" content="You can run .SH or Shell Script files in Windows 10 either using Windows Subsystem on Linux or install Ubuntu and then execute the scripts."/>
<meta property="og:url" content="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10"/>
<meta property="og:site_name" content="The Windows Club"/>
<meta property="og:updated_time" content="2020-07-05T12:30:50+05:30"/>
<meta property="article:publisher" content="https://www.facebook.com/TheWindowsClub/"/>
<meta property="og:image" content="https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Shell-script-files-from-Command-Prompt.png"/>
<meta property="og:image:width" content="600"/>
<meta property="og:image:height" content="295"/>
<meta property="article:published_time" content="2019-07-15T03:19:54+05:30"/>
<meta property="article:modified_time" content="2020-07-05T12:30:50+05:30"/>
<meta property="fb:app_id" content="1923155921341058"/>
<meta name="twitter:card" content="summary"/>
<meta name="twitter:title" content="How to run .sh or Shell Script file in Windows 10"/>
<meta name="twitter:description" content="You can run .SH or Shell Script files in Windows 10 either using Windows Subsystem on Linux or install Ubuntu and then execute the scripts."/>
<meta name="twitter:image:src" content="https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Shell-script-files-from-Command-Prompt.png"/>
<meta name="twitter:site" content="@TheWindowsClub"/>
<!-- Powered by Social Snap v1.1.15 - https://socialsnap.com/ -->


	<!-- This site is optimized with the Yoast SEO Premium plugin v15.9 - https://yoast.com/wordpress/plugins/seo/ -->
	<title>How to run .sh or Shell Script file in Windows 10</title>
	<meta name="description" content="You can run .SH or Shell Script files in Windows 10 either using Windows Subsystem on Linux or install Ubuntu and then execute the scripts."/>
	<meta name="robots" content="index, follow, max-snippet:-1, max-image-preview:large, max-video-preview:-1"/>
	<link rel="canonical" href="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10"/>
	<meta property="og:locale" content="en_US"/>
	<meta property="og:type" content="article"/>
	<meta property="og:title" content="How to run .sh or Shell Script file in Windows 10"/>
	<meta property="og:description" content="You can run .SH or Shell Script files in Windows 10 either using Windows Subsystem on Linux or install Ubuntu and then execute the scripts."/>
	<meta property="og:url" content="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10"/>
	<meta property="og:site_name" content="The Windows Club"/>
	<meta property="article:publisher" content="https://www.facebook.com/TheWindowsClub"/>
	<meta property="article:published_time" content="2019-07-14T21:49:54+00:00"/>
	<meta property="article:modified_time" content="2020-07-05T07:00:50+00:00"/>
	<meta property="og:image" content="https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Shell-script-files-from-Command-Prompt.png"/>
	<meta property="og:image:width" content="600"/>
	<meta property="og:image:height" content="295"/>
	<meta name="twitter:card" content="summary_large_image"/>
	<meta name="twitter:creator" content="@TheWindowsClub"/>
	<meta name="twitter:site" content="@TheWindowsClub"/>
	<meta property="og:video" content="https://www.youtube.com/embed/06E5etw4sqk"/>
	<meta property="og:video:type" content="text/html"/>
	<meta property="og:video:duration" content="247"/>
	<meta property="og:video:width" content="480"/>
	<meta property="og:video:height" content="270"/>
	<meta property="ya:ovs:adult" content="false"/>
	<meta property="ya:ovs:upload_date" content="2019-07-14T21:49:54+00:00"/>
	<meta property="ya:ovs:allow_embed" content="true"/>
	<!-- / Yoast SEO Premium plugin. -->


<link rel="dns-prefetch" href="//cdn.bibblio.org"/>
<link rel="dns-prefetch" href="//s.w.org"/>
<link rel="alternate" type="application/rss+xml" title="The Windows Club » Feed" href="https://www.thewindowsclub.com/feed"/>
<link rel="alternate" type="application/rss+xml" title="The Windows Club » Comments Feed" href="https://www.thewindowsclub.com/comments/feed"/>
<link rel="alternate" type="application/rss+xml" title="The Windows Club » How to run .sh or Shell Script file in Windows 10 Comments Feed" href="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10/feed"/>
		<script type="text/javascript">
			window._wpemojiSettings = {"baseUrl":"https:\/\/s.w.org\/images\/core\/emoji\/13.0.1\/72x72\/","ext":".png","svgUrl":"https:\/\/s.w.org\/images\/core\/emoji\/13.0.1\/svg\/","svgExt":".svg","source":{"concatemoji":"https:\/\/www.thewindowsclub.com\/wp-includes\/js\/wp-emoji-release.min.js?ver=5.6.2"}};
			!function(e,a,t){var n,r,o,i=a.createElement("canvas"),p=i.getContext&&i.getContext("2d");function s(e,t){var a=String.fromCharCode;p.clearRect(0,0,i.width,i.height),p.fillText(a.apply(this,e),0,0);e=i.toDataURL();return p.clearRect(0,0,i.width,i.height),p.fillText(a.apply(this,t),0,0),e===i.toDataURL()}function c(e){var t=a.createElement("script");t.src=e,t.defer=t.type="text/javascript",a.getElementsByTagName("head")[0].appendChild(t)}for(o=Array("flag","emoji"),t.supports={everything:!0,everythingExceptFlag:!0},r=0;r<o.length;r++)t.supports[o[r]]=function(e){if(!p||!p.fillText)return!1;switch(p.textBaseline="top",p.font="600 32px Arial",e){case"flag":return s([127987,65039,8205,9895,65039],[127987,65039,8203,9895,65039])?!1:!s([55356,56826,55356,56819],[55356,56826,8203,55356,56819])&&!s([55356,57332,56128,56423,56128,56418,56128,56421,56128,56430,56128,56423,56128,56447],[55356,57332,8203,56128,56423,8203,56128,56418,8203,56128,56421,8203,56128,56430,8203,56128,56423,8203,56128,56447]);case"emoji":return!s([55357,56424,8205,55356,57212],[55357,56424,8203,55356,57212])}return!1}(o[r]),t.supports.everything=t.supports.everything&&t.supports[o[r]],"flag"!==o[r]&&(t.supports.everythingExceptFlag=t.supports.everythingExceptFlag&&t.supports[o[r]]);t.supports.everythingExceptFlag=t.supports.everythingExceptFlag&&!t.supports.flag,t.DOMReady=!1,t.readyCallback=function(){t.DOMReady=!0},t.supports.everything||(n=function(){t.readyCallback()},a.addEventListener?(a.addEventListener("DOMContentLoaded",n,!1),e.addEventListener("load",n,!1)):(e.attachEvent("onload",n),a.attachEvent("onreadystatechange",function(){"complete"===a.readyState&&t.readyCallback()})),(n=t.source||{}).concatemoji?c(n.concatemoji):n.wpemoji&&n.twemoji&&(c(n.twemoji),c(n.wpemoji)))}(window,document,window._wpemojiSettings);
		</script>
		<style type="text/css">
img.wp-smiley,
img.emoji {
	display: inline !important;
	border: none !important;
	box-shadow: none !important;
	height: 1em !important;
	width: 1em !important;
	margin: 0 .07em !important;
	vertical-align: -0.1em !important;
	background: none !important;
	padding: 0 !important;
}
</style>
	<link rel="stylesheet" id="wp-block-library-css" href="https://www.thewindowsclub.com/wp-includes/css/dist/block-library/style.min.css?ver=5.6.2" type="text/css" media="all"/>
<link rel="stylesheet" id="bibblio_related_posts-css" href="https://www.thewindowsclub.com/wp-content/plugins/bibblio-related-posts/public/css/bibblio_related_posts-public.css?ver=1.3.7" type="text/css" media="all"/>
<link rel="stylesheet" id="bibblio-rcm-css-css" href="//cdn.bibblio.org/rcm/4.6/bib-related-content.css?ver=5.6.2" type="text/css" media="all"/>
<link rel="stylesheet" id="socialsnap-styles-css" href="https://www.thewindowsclub.com/wp-content/plugins/socialsnap-pro/assets/css/socialsnap.css?ver=1.1.15" type="text/css" media="all"/>
<link crossorigin="anonymous" rel="stylesheet" id="noozbeat-google-font-css" href="//fonts.googleapis.com/css?family=Open%2BSans%3A400%2C400italic%2C700%7CRoboto%3A400%2C700%26subset%3Dlatin%2Cgreek%2Cvietnamese%2Ccyrillic&amp;ver=5.6.2" type="text/css" media="all"/>
<link rel="stylesheet" id="noozbeat-base-css" href="https://www.thewindowsclub.com/wp-content/themes/noozbeat/css/base.css?ver=1.0" type="text/css" media="all"/>
<link rel="stylesheet" id="noozbeat-common-css" href="https://www.thewindowsclub.com/wp-content/themes/noozbeat/common/css/global.css?ver=1.0" type="text/css" media="all"/>
<link rel="stylesheet" id="flexslider-css" href="https://www.thewindowsclub.com/wp-content/themes/noozbeat/css/flexslider.css?ver=2.5.0" type="text/css" media="all"/>
<link rel="stylesheet" id="mmenu-css" href="https://www.thewindowsclub.com/wp-content/themes/noozbeat/css/mmenu.css?ver=5.2.0" type="text/css" media="all"/>
<link rel="stylesheet" id="font-awesome-css" href="https://www.thewindowsclub.com/wp-content/themes/noozbeat/css/font-awesome.css?ver=4.7.0" type="text/css" media="all"/>
<link rel="stylesheet" id="magnific-popup-css" href="https://www.thewindowsclub.com/wp-content/themes/noozbeat/css/magnific.css?ver=1.0.0" type="text/css" media="all"/>
<link rel="stylesheet" id="noozbeat-style-css" href="https://www.thewindowsclub.com/wp-content/themes/noozbeat/style.css?ver=1.0" type="text/css" media="all"/>
<link rel="stylesheet" id="noozbeat-style-child-css" href="https://www.thewindowsclub.com/wp-content/themes/noozbeat-child/style.css?ver=1.0" type="text/css" media="all"/>
<link rel="stylesheet" id="jquery-lazyloadxt-fadein-css-css" href="//www.thewindowsclub.com/wp-content/plugins/a3-lazy-load/assets/css/jquery.lazyloadxt.fadein.css?ver=5.6.2" type="text/css" media="all"/>
<link rel="stylesheet" id="a3a3_lazy_load-css" href="//www.thewindowsclub.com/wp-content/uploads/sass/a3_lazy_load.min.css?ver=1603042519" type="text/css" media="all"/>
<script type="text/javascript" src="https://www.thewindowsclub.com/wp-includes/js/jquery/jquery.min.js?ver=3.5.1" id="jquery-core-js"></script>
<script type="text/javascript" src="https://www.thewindowsclub.com/wp-includes/js/jquery/jquery-migrate.min.js?ver=3.3.2" id="jquery-migrate-js"></script>
<script type="text/javascript" src="https://www.thewindowsclub.com/wp-content/plugins/bibblio-related-posts/public/js/bibblio_related_posts-public.js?ver=1.3.7" id="bibblio_related_posts-js"></script>
<link rel="https://api.w.org/" href="https://www.thewindowsclub.com/wp-json/"/><link rel="alternate" type="application/json" href="https://www.thewindowsclub.com/wp-json/wp/v2/posts/186120"/><link rel="EditURI" type="application/rsd+xml" title="RSD" href="https://www.thewindowsclub.com/xmlrpc.php?rsd"/>
<link rel="wlwmanifest" type="application/wlwmanifest+xml" href="https://www.thewindowsclub.com/wp-includes/wlwmanifest.xml"/> 
<meta name="generator" content="WordPress 5.6.2"/>
<link rel="shortlink" href="https://www.thewindowsclub.com/?p=186120"/>
<link rel="alternate" type="application/json+oembed" href="https://www.thewindowsclub.com/wp-json/oembed/1.0/embed?url=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10"/>
<link rel="alternate" type="text/xml+oembed" href="https://www.thewindowsclub.com/wp-json/oembed/1.0/embed?url=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10&amp;format=xml"/>
<script type="text/javascript">//<![CDATA[
  function external_links_in_new_windows_loop() {
    if (!document.links) {
      document.links = document.getElementsByTagName('a');
    }
    var change_link = false;
    var force = '';
    var ignore = '';

    for (var t=0; t<document.links.length; t++) {
      var all_links = document.links[t];
      change_link = false;
      
      if(document.links[t].hasAttribute('onClick') == false) {
        // forced if the address starts with http (or also https), but does not link to the current domain
        if(all_links.href.search(/^http/) != -1 && all_links.href.search('www.thewindowsclub.com') == -1 && all_links.href.search(/^#/) == -1) {
          // console.log('Changed ' + all_links.href);
          change_link = true;
        }
          
        if(force != '' && all_links.href.search(force) != -1) {
          // forced
          // console.log('force ' + all_links.href);
          change_link = true;
        }
        
        if(ignore != '' && all_links.href.search(ignore) != -1) {
          // console.log('ignore ' + all_links.href);
          // ignored
          change_link = false;
        }

        if(change_link == true) {
          // console.log('Changed ' + all_links.href);
          document.links[t].setAttribute('onClick', 'javascript:window.open(\''+all_links.href+'\'); return false;');
          document.links[t].removeAttribute('target');
        }
      }
    }
  }
  
  // Load
  function external_links_in_new_windows_load(func)
  {  
    var oldonload = window.onload;
    if (typeof window.onload != 'function'){
      window.onload = func;
    } else {
      window.onload = function(){
        oldonload();
        func();
      }
    }
  }

  external_links_in_new_windows_load(external_links_in_new_windows_loop);
  //]]></script>

<script>
			document.addEventListener( "DOMContentLoaded", function() {
				var div, i,
					youtubePlayers = document.getElementsByClassName( "video-seo-youtube-player" );
				for ( i = 0; i < youtubePlayers.length; i++ ) {
					div = document.createElement( "div" );
					div.className = "video-seo-youtube-embed-loader";
					div.setAttribute( "data-id", youtubePlayers[ i ].dataset.id );
					div.setAttribute( "tabindex", "0" );
					div.setAttribute( "role", "button" );
					div.setAttribute( "aria-label", "Load YouTube video" );
					div.innerHTML = videoSEOGenerateYouTubeThumbnail( youtubePlayers[ i ].dataset.id );
					div.addEventListener( "click", videoSEOGenerateYouTubeIframe );
					div.addEventListener( "keydown", videoSEOYouTubeThumbnailHandleKeydown );
					div.addEventListener( "keyup", videoSEOYouTubeThumbnailHandleKeyup );
					youtubePlayers[ i ].appendChild( div );
				}
			} );

			function videoSEOGenerateYouTubeThumbnail( id ) {
				var thumbnail = '<picture class="video-seo-youtube-picture">\n' +
					'<source class="video-seo-source-to-maybe-replace" media="(min-width: 801px)" srcset="https://i.ytimg.com/vi/' + id + '/maxresdefault.jpg" >\n' +
					'<source class="video-seo-source-hq" media="(max-width: 800px)" srcset="https://i.ytimg.com/vi/' + id + '/hqdefault.jpg">\n' +
					'<img onload="videoSEOMaybeReplaceMaxResSourceWithHqSource( event );" src="https://i.ytimg.com/vi/' + id + '/hqdefault.jpg" width="480" height="360" loading="eager" alt="">\n' +
					'</picture>\n',
					play = '<div class="video-seo-youtube-player-play"></div>';
				return thumbnail.replace( "ID", id ) + play;
			}

			function videoSEOMaybeReplaceMaxResSourceWithHqSource( event ) {
				var sourceMaxRes,
					sourceHighQuality,
					loadedThumbnail = event.target,
					parent = loadedThumbnail.parentNode;

				if ( loadedThumbnail.naturalWidth < 150 ) {
					sourceMaxRes = parent.querySelector(".video-seo-source-to-maybe-replace");
					sourceHighQuality = parent.querySelector(".video-seo-source-hq");
					sourceMaxRes.srcset = sourceHighQuality.srcset;
					parent.className = "video-seo-youtube-picture video-seo-youtube-picture-replaced-srcset";
				}
			}

			function videoSEOYouTubeThumbnailHandleKeydown( event ) {
				if ( event.keyCode !== 13 && event.keyCode !== 32 ) {
					return;
				}

				if ( event.keyCode === 13 ) {
					videoSEOGenerateYouTubeIframe( event );
				}

				if ( event.keyCode === 32 ) {
					event.preventDefault();
				}
			}

			function videoSEOYouTubeThumbnailHandleKeyup( event ) {
				if ( event.keyCode !== 32 ) {
					return;
				}

				videoSEOGenerateYouTubeIframe( event );
			}

			function videoSEOGenerateYouTubeIframe( event ) {
				var el = ( event.type === "click" ) ? this : event.target,
					iframe = document.createElement( "iframe" );

				iframe.setAttribute( "src", "https://www.youtube.com/embed/" + el.dataset.id + "?autoplay=1&enablejsapi=1&origin=https%3A%2F%2Fwww.thewindowsclub.com" );
				iframe.setAttribute( "frameborder", "0" );
				iframe.setAttribute( "allowfullscreen", "1" );
				iframe.setAttribute( "allow", "accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" );
				el.parentNode.replaceChild( iframe, el );
			}
		</script><style type="text/css">			.foot {
				background-color: #ffffff;
			}
						.sidebar a,
			.sidebar a:hover {
				color: #1e73be;
			}
						.sidebar a:hover {
				color: #0568bf;
			}
						h1:not(.site-logo) {
				font-size: 36px;
			}
						body,
			.entry-content {
				font-size: 16px;
			}
			</style>
<!-- Schema & Structured Data For WP v1.9.65 - -->
<script type="application/ld+json" class="saswp-schema-markup-output">
[{"@context":"https:\/\/schema.org","@graph":[{"@context":"https:\/\/schema.org","@type":"SiteNavigationElement","@id":"https:\/\/www.thewindowsclub.com\/#Main_Menu","name":"Home","url":"https:\/\/www.thewindowsclub.com"},{"@context":"https:\/\/schema.org","@type":"SiteNavigationElement","@id":"https:\/\/www.thewindowsclub.com\/#Main_Menu","name":"Windows","url":"https:\/\/www.thewindowsclub.com\/category\/windows"},{"@context":"https:\/\/schema.org","@type":"SiteNavigationElement","@id":"https:\/\/www.thewindowsclub.com\/#Main_Menu","name":"Downloads","url":"https:\/\/www.thewindowsclub.com\/category\/downloads"},{"@context":"https:\/\/schema.org","@type":"SiteNavigationElement","@id":"https:\/\/www.thewindowsclub.com\/#Main_Menu","name":"Security","url":"https:\/\/www.thewindowsclub.com\/category\/security"},{"@context":"https:\/\/schema.org","@type":"SiteNavigationElement","@id":"https:\/\/www.thewindowsclub.com\/#Main_Menu","name":"Office","url":"https:\/\/www.thewindowsclub.com\/category\/office"},{"@context":"https:\/\/schema.org","@type":"SiteNavigationElement","@id":"https:\/\/www.thewindowsclub.com\/#Main_Menu","name":"General","url":"https:\/\/www.thewindowsclub.com\/category\/general"},{"@context":"https:\/\/schema.org","@type":"SiteNavigationElement","@id":"https:\/\/www.thewindowsclub.com\/#Main_Menu","name":"News","url":"https:\/\/news.thewindowsclub.com"},{"@context":"https:\/\/schema.org","@type":"SiteNavigationElement","@id":"https:\/\/www.thewindowsclub.com\/#Main_Menu","name":"Reviews","url":"https:\/\/reviews.thewindowsclub.com\/"},{"@context":"https:\/\/schema.org","@type":"SiteNavigationElement","@id":"https:\/\/www.thewindowsclub.com\/#Main_Menu","name":"About","url":"https:\/\/www.thewindowsclub.com\/about"}]},

{"@context":"https:\/\/schema.org","@type":"BlogPosting","@id":"https:\/\/www.thewindowsclub.com\/how-to-run-sh-or-shell-script-file-in-windows-10\/#BlogPosting","url":"https:\/\/www.thewindowsclub.com\/how-to-run-sh-or-shell-script-file-in-windows-10\/","inLanguage":"en-US","mainEntityOfPage":"https:\/\/www.thewindowsclub.com\/how-to-run-sh-or-shell-script-file-in-windows-10\/","headline":"How to run .sh or Shell Script file in Windows 10","description":"You can run .SH or Shell Script files in Windows 10 either using Windows Subsystem on Linux or install Ubuntu and then execute the scripts.","articleBody":"Shell Scripts or .SH files are like batch files of Windows which can be executed in Linux or Unix. It is possible to run .sh or Shell Script file in Windows 10 using Windows Subsystem for Linux. In this post, we will show you how to run a Shell Script file in Windows 10.  How to run .sh or Shell Script file in Windows 10  Bash\u00a0is a\u00a0Unix shell\u00a0and\u00a0command language which can run Shell Script files. You do not need to install Ubuntu or any other Linux Distros unless your scripts need the support of the real Linux kernel. We will share both the methods.     \tExecute Shell Script file using WSL   \tExecute Shell Script using Ubuntu on Windows 10    1] Execute Shell Script file using WSL  Install WSL or Windows Subsystem for Linux    Go to\u00a0Settings &gt; Update &amp; Security &gt; For Developers. Check the\u00a0Developer Mode\u00a0radio button. And search for \u201cWindows Features\u201d, choose \u201cTurn Windows features on or off\u201d.    Scroll to find WSL, check the box, and then install it. Once done, one has to reboot to finish installing the requested changes. Press Restart now.\u00a0 BASH will be available in the Command Prompt and PowerShell.    Execute Shell Script Files     \tOpen Command Prompt and navigate to the folder where the script file is available.   \tType Bash script-filename.sh and hit the enter key.   \tIt will execute the script, and depending on the file, you should see an output.        On a Linux platform, you usually use SH, but here you need to use BASH. That said, BASH in Windows has its limitations, so if you want to execute in a Linux environment, you need to install Ubuntu or anything similar.    https:\/\/youtu.be\/06E5etw4sqk  2] Execute Shell Script using Ubuntu on Windows 10  Make sure you have Ubuntu or any other Linux distros installed.\u00a0 Ubuntu will mount or make all your Windows directories available under \/mnt. So the C drive is available at \/mnt\/C.\u00a0 So if the desktop will be available at \/mnt\/c\/users\/&lt;username&gt;\/desktop.        Now follow these steps     \tType Bash in run prompt, and it will launch the distro prompt.   \tNavigate to the folder using \"cd\" command to the folder where the scripts are available.   \tType \"sh script.sh\" and hit enter.    It will execute the script, and if they have a dependency on any of core Linux features.    Since Linux is now available in Windows, you need not use any third party applications like Cygwin. WSL should be enough for most of the scenarios to help you run a shell script in Windows 10.","keywords":"WSL, ","name":"How to run .sh or Shell Script file in Windows 10","datePublished":"2019-07-15T03:19:54+05:30","dateModified":"2020-07-05T12:30:50+05:30","author":{"@type":"Person","name":"AshishMohta@TWC","description":"Ashish is a veteran Windows, and Xbox user who excels in writing tips, tricks, and features on it to improve your day to day experience with your devices.","url":"https:\/\/www.thewindowsclub.com\/author\/ash5moh8twc","sameAs":[],"image":{"@type":"ImageObject","url":"https:\/\/secure.gravatar.com\/avatar\/fb6d7213911a177d3cb4af07eac30fdc?s=96&r=g","height":96,"width":96}},"publisher":{"@type":"Organization","name":"TheWindowsClub","url":"https:\/\/www.thewindowsclub.com","logo":{"@type":"ImageObject","url":"https:\/\/www.thewindowsclub.com\/wp-content\/uploads\/2020\/01\/TheWindowsClub.png","width":"510","height":"60"}},"image":[{"@type":"ImageObject","@id":"https:\/\/www.thewindowsclub.com\/how-to-run-sh-or-shell-script-file-in-windows-10#primaryimage","url":"https:\/\/www.thewindowsclub.com\/wp-content\/uploads\/2019\/07\/Run-Shell-script-files-from-Command-Prompt-1200x900.png","width":"1200","height":"900"},{"@type":"ImageObject","url":"https:\/\/www.thewindowsclub.com\/wp-content\/uploads\/2019\/07\/Run-Shell-script-files-from-Command-Prompt-1200x720.png","width":"1200","height":"720"},{"@type":"ImageObject","url":"https:\/\/www.thewindowsclub.com\/wp-content\/uploads\/2019\/07\/Run-Shell-script-files-from-Command-Prompt-1200x675.png","width":"1200","height":"675"},{"@type":"ImageObject","url":"https:\/\/www.thewindowsclub.com\/wp-content\/uploads\/2019\/07\/Run-Shell-script-files-from-Command-Prompt-600x295.png","width":600,"height":295},{"@type":"ImageObject","url":"https:\/\/www.thewindowsclub.com\/wp-content\/uploads\/2019\/07\/Run-Script-files-in-Windows-via-Ubuntu-600x187.png","width":600,"height":187}]},

{"@context":"https:\/\/schema.org","@type":"BlogPosting","@id":"https:\/\/www.thewindowsclub.com\/how-to-run-sh-or-shell-script-file-in-windows-10\/#BlogPosting","url":"https:\/\/www.thewindowsclub.com\/how-to-run-sh-or-shell-script-file-in-windows-10\/","inLanguage":"en-US","mainEntityOfPage":"https:\/\/www.thewindowsclub.com\/how-to-run-sh-or-shell-script-file-in-windows-10\/","headline":"How to run .sh or Shell Script file in Windows 10","description":"You can run .SH or Shell Script files in Windows 10 either using Windows Subsystem on Linux or install Ubuntu and then execute the scripts.","articleBody":"Shell Scripts or .SH files are like batch files of Windows which can be executed in Linux or Unix. It is possible to run .sh or Shell Script file in Windows 10 using Windows Subsystem for Linux. In this post, we will show you how to run a Shell Script file in Windows 10.  How to run .sh or Shell Script file in Windows 10  Bash\u00a0is a\u00a0Unix shell\u00a0and\u00a0command language which can run Shell Script files. You do not need to install Ubuntu or any other Linux Distros unless your scripts need the support of the real Linux kernel. We will share both the methods.     \tExecute Shell Script file using WSL   \tExecute Shell Script using Ubuntu on Windows 10    1] Execute Shell Script file using WSL  Install WSL or Windows Subsystem for Linux    Go to\u00a0Settings &gt; Update &amp; Security &gt; For Developers. Check the\u00a0Developer Mode\u00a0radio button. And search for \u201cWindows Features\u201d, choose \u201cTurn Windows features on or off\u201d.    Scroll to find WSL, check the box, and then install it. Once done, one has to reboot to finish installing the requested changes. Press Restart now.\u00a0 BASH will be available in the Command Prompt and PowerShell.    Execute Shell Script Files     \tOpen Command Prompt and navigate to the folder where the script file is available.   \tType Bash script-filename.sh and hit the enter key.   \tIt will execute the script, and depending on the file, you should see an output.        On a Linux platform, you usually use SH, but here you need to use BASH. That said, BASH in Windows has its limitations, so if you want to execute in a Linux environment, you need to install Ubuntu or anything similar.    https:\/\/youtu.be\/06E5etw4sqk  2] Execute Shell Script using Ubuntu on Windows 10  Make sure you have Ubuntu or any other Linux distros installed.\u00a0 Ubuntu will mount or make all your Windows directories available under \/mnt. So the C drive is available at \/mnt\/C.\u00a0 So if the desktop will be available at \/mnt\/c\/users\/&lt;username&gt;\/desktop.        Now follow these steps     \tType Bash in run prompt, and it will launch the distro prompt.   \tNavigate to the folder using \"cd\" command to the folder where the scripts are available.   \tType \"sh script.sh\" and hit enter.    It will execute the script, and if they have a dependency on any of core Linux features.    Since Linux is now available in Windows, you need not use any third party applications like Cygwin. WSL should be enough for most of the scenarios to help you run a shell script in Windows 10.","keywords":"WSL, ","name":"How to run .sh or Shell Script file in Windows 10","datePublished":"2019-07-15T03:19:54+05:30","dateModified":"2020-07-05T12:30:50+05:30","author":{"@type":"Person","name":"AshishMohta@TWC","description":"Ashish is a veteran Windows, and Xbox user who excels in writing tips, tricks, and features on it to improve your day to day experience with your devices.","url":"https:\/\/www.thewindowsclub.com\/author\/ash5moh8twc","sameAs":[],"image":{"@type":"ImageObject","url":"https:\/\/secure.gravatar.com\/avatar\/fb6d7213911a177d3cb4af07eac30fdc?s=96&r=g","height":96,"width":96}},"publisher":{"@type":"Organization","name":"TheWindowsClub","url":"https:\/\/www.thewindowsclub.com","logo":{"@type":"ImageObject","url":"https:\/\/www.thewindowsclub.com\/wp-content\/uploads\/2020\/01\/TheWindowsClub.png","width":"510","height":"60"}},"image":[{"@type":"ImageObject","@id":"https:\/\/www.thewindowsclub.com\/how-to-run-sh-or-shell-script-file-in-windows-10#primaryimage","url":"https:\/\/www.thewindowsclub.com\/wp-content\/uploads\/2019\/07\/Run-Shell-script-files-from-Command-Prompt-1200x900.png","width":"1200","height":"900"},{"@type":"ImageObject","url":"https:\/\/www.thewindowsclub.com\/wp-content\/uploads\/2019\/07\/Run-Shell-script-files-from-Command-Prompt-1200x720.png","width":"1200","height":"720"},{"@type":"ImageObject","url":"https:\/\/www.thewindowsclub.com\/wp-content\/uploads\/2019\/07\/Run-Shell-script-files-from-Command-Prompt-1200x675.png","width":"1200","height":"675"},{"@type":"ImageObject","url":"https:\/\/www.thewindowsclub.com\/wp-content\/uploads\/2019\/07\/Run-Shell-script-files-from-Command-Prompt-600x295.png","width":600,"height":295},{"@type":"ImageObject","url":"https:\/\/www.thewindowsclub.com\/wp-content\/uploads\/2019\/07\/Run-Script-files-in-Windows-via-Ubuntu-600x187.png","width":600,"height":187}]}]
</script>

<link rel="amphtml" href="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10/amp"/><link rel="icon" href="https://www.thewindowsclub.com/wp-content/uploads/2020/01/cropped-TheWindowsClub-Icon-32x32.png" sizes="32x32"/>
<link rel="icon" href="https://www.thewindowsclub.com/wp-content/uploads/2020/01/cropped-TheWindowsClub-Icon-192x192.png" sizes="192x192"/>
<link rel="apple-touch-icon" href="https://www.thewindowsclub.com/wp-content/uploads/2020/01/cropped-TheWindowsClub-Icon-180x180.png"/>
<meta name="msapplication-TileImage" content="https://www.thewindowsclub.com/wp-content/uploads/2020/01/cropped-TheWindowsClub-Icon-270x270.png"/>
		<style type="text/css" id="wp-custom-css">
			/* Hyperlink MarkerUnderline */
.y-link-underline a {
    border-bottom: 1px solid #B4E7F8;
    box-shadow: 0 -2px 0 #B4E7F8 inset;
    color: inherit;
    transition: background 0.15s cubic-bezier(0.33, 0.66, 0.66, 1) 0s;
}
.y-link-underline a:hover, .link-underline a:focus, .link-underline a:active {
    background: none repeat scroll 0 0 #B4E7F8;
    color: inherit;
    text-decoration:none;
}

/* Logo Center Align */
.head-wrap .head-wrap-col-left {
    width: 100%;
    text-align: center;
}
.head-wrap .head-wrap-col-right {
    display: none;
}
.entry-related img {
    height: 116px;
    width: auto;
    margin: auto;
    display: block;
}

/* Advt Visiblity Mobile or Desktop */
.mobileHide { display: inline;}
   /* Smartphone Portrait and Landscape */
   @media only screen and (min-device-width : 320px)
   and (max-device-width : 480px){  .mobileHide { display: none;}}
		</style>
		<style>.ezoic-ad.box-2894 { display:block !important;float:none;line-height:0px;margin-bottom:15px !important;margin-left:0px !important;margin-right:0px !important;margin-top:15px !important;min-height:90px;min-width:728px;text-align:center !important; }
.ezoic-ad.box-3144 { display:block !important;float:none !important;line-height:0px;margin-bottom:0px !important;margin-left:0px !important;margin-right:0px !important;margin-top:0px !important;min-height:250px;min-width:300px;text-align:center !important; }
.ezoic-ad.medrectangle-3153 { display:block !important;float:none !important;line-height:0px;margin-bottom:0px !important;margin-left:0px !important;margin-right:0px !important;margin-top:0px !important;min-height:400px;min-width:580px;text-align:center !important; }
.ezoic-ad.medrectangle-4600 { display:block !important;float:none !important;line-height:0px;margin-bottom:0px !important;margin-left:0px !important;margin-right:0px !important;margin-top:0px !important;min-height:250px;min-width:300px;text-align:center !important; }
.ezoic-ad.large-mobile-banner-1105 { display:block !important;float:none !important;line-height:0px;margin-bottom:15px !important;margin-left:0px !important;margin-right:0px !important;margin-top:15px !important;min-height:400px;min-width:580px;text-align:center !important; }
.ezoic-ad.box-1870 { display:block !important;float:none;line-height:0px;margin-bottom:15px !important;margin-left:0px !important;margin-right:0px !important;margin-top:15px !important;min-height:280px;min-width:336px;text-align:center !important; }
.ezoic-ad.banner-2104 { display:block !important;float:none !important;line-height:0px;margin-bottom:15px !important;margin-left:0px !important;margin-right:0px !important;margin-top:15px !important;min-height:600px;min-width:300px;text-align:center !important; }
.ezoic-ad.medrectangle-1121 { display:block !important;float:left !important;line-height:0px;margin-bottom:15px !important;margin-left:0px !important;margin-right:0px !important;margin-top:15px !important;min-height:90px;min-width:728px;text-align:center !important; }
.ezoic-ad{display:inline-block;line-height:0px;border:0px;}
.adtester-container-823,.adtester-container-142,.adtester-container-184,.adtester-container-832,.adtester-container-835,.adtester-container-880,.adtester-container-193,.adtester-container-149,.adtester-container-186,.adtester-container-824,.adtester-container-125,.adtester-container-678,.adtester-container-194,.adtester-container-183,.adtester-container-619,.adtester-container-176,.adtester-container-860,.adtester-container-843,.adtester-container-834,.adtester-container-102,.adtester-container-637,.adtester-container-686,.adtester-container-141,.adtester-container-146,.adtester-container-192,.adtester-container-602,.adtester-container-885,.adtester-container-874,.adtester-container-840,.adtester-container-846,.adtester-container-103,.adtester-container-676,.adtester-container-608,.adtester-container-147,.adtester-container-808,.adtester-container-114,.adtester-container-151,.adtester-container-630,.adtester-container-613,.adtester-container-652,.adtester-container-887,.adtester-container-164,.adtester-container-116,.adtester-container-604,.adtester-container-828,.adtester-container-163,.adtester-container-800,.adtester-container-661,.adtester-container-177,.adtester-container-879,.adtester-container-666,.adtester-container-864,.adtester-container-197,.adtester-container-106,.adtester-container-875,.adtester-container-656,.adtester-container-614,.adtester-container-673,.adtester-container-156,.adtester-container-627,.adtester-container-896,.adtester-container-601,.adtester-container-675,.adtester-container-135,.adtester-container-603,.adtester-container-624,.adtester-container-868,.adtester-container-195,.adtester-container-856,.adtester-container-849,.adtester-container-825,.adtester-container-158,.adtester-container-845,.adtester-container-817,.adtester-container-133,.adtester-container-150,.adtester-container-180,.adtester-container-136,.adtester-container-110,.adtester-container-166,.adtester-container-830,.adtester-container-625,.adtester-container-689,.adtester-container-818,.adtester-container-612,.adtester-container-119,.adtester-container-108,.adtester-container-178,.adtester-container-855,.adtester-container-179,.adtester-container-623,.adtester-container-618,.adtester-container-120,.adtester-container-616,.adtester-container-859,.adtester-container-113,.adtester-container-615,.adtester-container-653,.adtester-container-172,.adtester-container-886,.adtester-container-189,.adtester-container-629,.adtester-container-127,.adtester-container-148,.adtester-container-155,.adtester-container-609,.adtester-container-813,.adtester-container-123,.adtester-container-199,.adtester-container-188,.adtester-container-862,.adtester-container-853,.adtester-container-858,.adtester-container-174,.adtester-container-159,.adtester-container-857,.adtester-container-662,.adtester-container-117,.adtester-container-107,.adtester-container-635,.adtester-container-182,.adtester-container-109,.adtester-container-165,.adtester-container-848,.adtester-container-621,.adtester-container-126,.adtester-container-622,.adtester-container-167,.adtester-container-611,.adtester-container-850,.adtester-container-605,.adtester-container-610,.adtester-container-617,.adtester-container-893,.adtester-container-854,.adtester-container-631,.adtester-container-693,.adtester-container-833,.adtester-container-187,.adtester-container-130,.adtester-container-190,.adtester-container-198,.adtester-container-160,.adtester-container-140,.adtester-container-888,.adtester-container-131,.adtester-container-154,.adtester-container-122,.adtester-container-145,.adtester-container-124,.adtester-container-684,.adtester-container-810,.adtester-container-841,.adtester-container-626,.adtester-container-827,.adtester-container-606,.adtester-container-651,.adtester-container-831,.adtester-container-175,.adtester-container-118,.adtester-container-844,.adtester-container-803,.adtester-container-143,.adtester-container-620,.adtester-container-168,.adtester-container-115,.adtester-container-837,.adtester-container-162,.adtester-container-838,.adtester-container-607,.adtester-container-152,.adtester-container-137,.adtester-container-181,.adtester-container-847,.adtester-container-852,.adtester-container-132,.adtester-container-809,.adtester-container-171,.adtester-container-866,.adtester-container-185,.adtester-container-112,.adtester-container-170,.adtester-container-863,.adtester-container-876,.adtester-container-851,.adtester-container-878,.adtester-container-169,.adtester-container-836,.adtester-container-173,.adtester-container-861,.adtester-container-157,.adtester-container-196,.adtester-container-191,.adtester-container-865,.adtester-container-161{display:none!important}
.ezoic-floating-bottom { display: none!important; }</style><script type="text/javascript">var ezouid = "1";</script><base href="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10"><script type='text/javascript'>
var ezoTemplate = 'pub_site';
if(typeof ezouid == 'undefined')
{
    var ezouid = 'none';
}
var ezoFormfactor = '1';
var ezo_elements_to_check = Array();
</script><!-- START EZHEAD -->
<script data-ezscrex="false" type='text/javascript'>
var soc_app_id = '0';
var did = 77472;
var ezdomain = 'thewindowsclub.com';
var ezoicSearchable = 1;
</script>
<!--{jquery}-->
<!-- END EZHEAD -->
<script data-ezscrex='false' data-cfasync='false' type='text/javascript' style='display:none' defer>__ez.queue.addFile('__ezf_ezosuigeneris', '//g.ezoic.net/ezosuigeneris.js?i=f2f240a440d92b9b80972d610bf00908', true, ["/detroitchicago/boise.js"], true, false, false, false);</script><script data-ezscrex='false' data-cfasync='false' type='text/javascript' style='display:none' defer>__ez.queue.addFile('__ezf_ezosuigenerisc', '//g.ezoic.net/ezosuigenerisc.js?i=5183c468409fc473806bb6879340fc3e', true, ["/detroitchicago/boise.js"], true, false, false, false);</script>
<script data-ezscrex='false' data-pagespeed-no-defer data-cfasync='false'>
function create_ezolpl(pvID, rv) {
    var d = new Date();
    d.setTime(d.getTime() + (365*24*60*60*1000));
    var expires = "expires="+d.toUTCString();
    __ez.ck.setByCat("ezux_lpl_77472=" + new Date().getTime() + "|" + pvID + "|" + rv + "; " + expires, 3);
}
function attach_ezolpl(pvID, rv) {
    if (document.readyState === "complete") {
        create_ezolpl(pvID, rv);
    }
    if(window.attachEvent) {
        window.attachEvent("onload", create_ezolpl, pvID, rv);
    } else {
        if(window.onload) {
            var curronload = window.onload;
            var newonload = function(evt) {
                curronload(evt);
                create_ezolpl(pvID, rv);
            };
            window.onload = newonload;
        } else {
            window.onload = create_ezolpl.bind(null, pvID, rv);
        }
    }
}

__ez.queue.addFunc("attach_ezolpl", "attach_ezolpl", ["c2eeeada-291f-4952-4ff1-a0e3639cb84d", "false"], false, ['/detroitchicago/boise.js'], true, false, false, false);
</script></head>
<body data-rsssl="1" class="post-template-default single single-post postid-186120 single-format-standard">

<div id="page">

<header class="header">
	
	<div class="mast-head">
		<div class="container">
			<div class="row">
				<div class="col-xs-12">
					<div class="head-wrap">
						<div class="head-wrap-col-left">
							<div class="site-logo">
								<a href="https://www.thewindowsclub.com/">
																			<img src="https://www.thewindowsclub.com/wp-content/uploads/2020/01/TheWindowsClub.png" alt="The Windows Club"/>
																	</a>

							</div>

							
						</div>

						<div class="head-wrap-col-right">
													</div>
					</div>

					<nav class="nav">
						<a href="#mobilemenu" class="mobile-trigger"><i class="fa fa-navicon"></i> MENU</a>

						<ul id="menu-main_menu" class="navigation"><li id="menu-item-13910" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-home menu-item-13910"><a href="https://www.thewindowsclub.com">Home</a></li>
<li id="menu-item-201599" class="menu-item menu-item-type-taxonomy menu-item-object-category current-post-ancestor current-menu-parent current-post-parent menu-item-201599"><a href="https://www.thewindowsclub.com/category/windows">Windows</a></li>
<li id="menu-item-13912" class="menu-item menu-item-type-taxonomy menu-item-object-category menu-item-13912"><a href="https://www.thewindowsclub.com/category/downloads">Downloads</a></li>
<li id="menu-item-13919" class="menu-item menu-item-type-taxonomy menu-item-object-category menu-item-13919"><a href="https://www.thewindowsclub.com/category/security">Security</a></li>
<li id="menu-item-13917" class="menu-item menu-item-type-taxonomy menu-item-object-category menu-item-13917"><a href="https://www.thewindowsclub.com/category/office">Office</a></li>
<li id="menu-item-201600" class="menu-item menu-item-type-taxonomy menu-item-object-category menu-item-201600"><a href="https://www.thewindowsclub.com/category/general">General</a></li>
<li id="menu-item-57949" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-57949"><a href="https://news.thewindowsclub.com">News</a></li>
<li id="menu-item-136107" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-136107"><a href="https://reviews.thewindowsclub.com/">Reviews</a></li>
<li id="menu-item-13911" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-13911"><a href="https://www.thewindowsclub.com/about">About</a></li>
</ul>            <form action="https://www.thewindowsclub.com/the-windows-club-search-results" class="searchform" method="get" role="search">
	<div>
		<label class="screen-reader-text">Search for:</label>
		<input name="cx" type="hidden" value="partner-pub-5950002284129980:7lz6cl-5ojg"/> 
		
		  <input name="cof" type="hidden" value="FORID:11"/> 
		  <input name="ie" type="hidden" value="ISO-8859-1"/>
		
		<input id="s" name="q" size="18" type="text" placeholder="Type and press enter" value=""/>
		<a class="btn searchsubmit"><i class="fa fa-search"></i></a>
	</div>
</form>
						
					</nav><!-- #nav -->

					<div id="mobilemenu"></div>
				</div>
			</div>
		</div>
	</div>
</header>



  
  
  <main class="main">
  	<div class="container">
  		<div class="row"><span id="ezoic-pub-ad-placeholder-803" class="ezoic-adpicker-ad"></span>
  
  			  

<div class="col-xs-12">

	
	
		<div class="entry-head "> <!-- add the class .text-center for a centered article header -->
							<div class="entry-meta">
					
											<time class="entry-time" datetime="2019-07-15T03:19:54+05:30">July 15, 2019</time>
									</div>
			
			<h1 class="entry-title">How to run .sh or Shell Script file in Windows 10</h1>
			
	<!-- Ezoic - top_of_page 894 - top_of_page -->
<span id="ezoic-pub-ad-placeholder-894"></span><span class='ezoic-ad box-2 box-2894 adtester-container adtester-container-894' data-ez-name='thewindowsclub_com-box-2'><span id='div-gpt-ad-thewindowsclub_com-box-2-0' ezaw='728' ezah='90' style='position:relative;z-index:0;display:inline-block;min-height:90px;min-width:728px;' class='ezoic-ad'><script data-ezscrex='false' data-cfasync='false' type='text/javascript' style='display:none;'>eval(ez_write_tag([[728,90],'thewindowsclub_com-box-2','ezslot_7',894,'0','0']));</script></span></span>
<!-- End Ezoic - top_of_page 894 - top_of_page -->

			<div class="entry-submeta">
												<!--  	<span class="entry-share">Share:				<a target="_blank" class="icon-social" href="https://www.facebook.com/sharer.php?u=https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10"><i class="fa fa-facebook"></i></a>
		<a target="_blank" class="icon-social" href="https://twitter.com/share?url=https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10"><i class="fa fa-twitter"></i></a>
					<a target="_blank" class="icon-social" href="https://pinterest.com/pin/create/bookmarklet/?url=https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10&description=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010&media=https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Shell-script-files-from-Command-Prompt-600x295.png"><i class="fa fa-pinterest"></i></a>
			</span>
 -->
			</div>
		</div><!-- .entry-head -->

	
	
			<div class="row">
			<div class="col-md-8 col-sm-12 col-xs-12">
	
			
								
<div class="y-link-underline">

<div class="entry-affiliate" align="center">
<strong><a href="http://www.restoro.com/includes/route.php?tracking=twc&amp;lpx=lwdu" rel="nofollow">Download this PC Repair Tool to quickly find &amp; fix Windows errors automatically</a></strong></div><!-- .entry-affiliate-End -->

				<div class="entry-content">
					
<!-- Quick Adsense WordPress Plugin: http://quickadsense.com/ -->
<div class="c24ff8f4a2da697123def04f69833d8b" data-index="4" style="float: none; margin:10px 0 10px 0; text-align:center;">

</div>
<p><strong>Shell Scripts</strong> or<strong> .SH files</strong> are like batch files of Windows which can be executed in Linux or Unix. It is possible to run .sh or Shell Script file in Windows 10 using Windows Subsystem for Linux. In this post, we will show you how to run a Shell Script file in Windows 10.<span id="ezoic-pub-ad-placeholder-679" class="ezoic-adpicker-ad"></span></p>
<h2>How to run .sh or Shell Script file in Windows 10</h2>
<p><b>Bash</b> is a Unix shell and command language which can run Shell Script files. You do not need to install Ubuntu or any other Linux Distros unless your scripts need the support of the real Linux kernel. We will share both the methods.</p>
<ol>
<li>Execute Shell Script file using WSL</li>
<li>Execute Shell Script using Ubuntu on Windows 10</li>
</ol>
<h3>1] Execute Shell Script file using WSL</h3>
<p><strong>Install WSL or Windows Subsystem for Linux</strong></p><div class="code-block code-block-16" style="margin: 8px 0; clear: both;">
<!-- Ezoic - under_3rd_para - under_page_title -->
<span id="ezoic-pub-ad-placeholder-624"></span>
<!-- End Ezoic - under_3rd_para - under_page_title --></div>

<p>Go to Settings &gt; Update &amp; Security &gt; For Developers. Check the <em>Developer Mode</em> radio button. And search for “<em>Windows Features</em>”, choose “<a href="https://www.thewindowsclub.com/ways-to-enable-or-disable-optional-windows-features"><em>Turn Windows features on or off</em></a>”.</p><div class="code-block code-block-1" style="margin: 8px 0; clear: both;">
<!-- Ezoic -  under_4th_para - under_page_title -->
<span id="ezoic-pub-ad-placeholder-141"></span>
<!-- End Ezoic -  under_4th_para - under_page_title --></div>

<p>Scroll to find WSL, check the box, and <a href="https://www.thewindowsclub.com/run-bash-on-windows-10">then install it</a>. Once done, one has to reboot to finish installing the requested changes. Press Restart now.  BASH will be available in the Command Prompt and PowerShell.</p><div class="code-block code-block-2" style="margin: 8px 0; clear: both;">
<!-- Ezoic - under_5th_para - under_page_title -->
<span id="ezoic-pub-ad-placeholder-144"></span><span class='ezoic-ad box-3 box-3144 adtester-container adtester-container-144' data-ez-name='thewindowsclub_com-box-3'><span id='div-gpt-ad-thewindowsclub_com-box-3-0' ezaw='300' ezah='250' style='position:relative;z-index:0;display:inline-block;min-height:250px;min-width:300px;' class='ezoic-ad'><script data-ezscrex='false' data-cfasync='false' type='text/javascript' style='display:none;'>eval(ez_write_tag([[300,250],'thewindowsclub_com-box-3','ezslot_0',144,'0','0']));</script></span></span>
<!-- End Ezoic - under_5th_para - under_page_title --></div>

<p><strong>Execute Shell Script Files</strong></p>
<ol>
<li>Open Command Prompt and navigate to the folder where the script file is available.</li>
<li>Type Bash script-filename.sh and hit the enter key.</li>
<li>It will execute the script, and depending on the file, you should see an output.</li>
</ol>
<p><img loading="lazy" class="lazy lazy-hidden aligncenter size-large wp-image-186225" src="//www.thewindowsclub.com/wp-content/plugins/a3-lazy-load/assets/images/lazy_placeholder.gif" data-lazy-type="image" data-src="https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Shell-script-files-from-Command-Prompt-600x295.png" alt="Run Shell script files from Command Prompt" width="600" height="295" srcset="" data-srcset="https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Shell-script-files-from-Command-Prompt.png 600w, https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Shell-script-files-from-Command-Prompt-150x74.png 150w, https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Shell-script-files-from-Command-Prompt-400x197.png 400w" sizes="(max-width: 600px) 100vw, 600px"/><noscript><img loading="lazy" class="aligncenter size-large wp-image-186225" src="https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Shell-script-files-from-Command-Prompt-600x295.png" alt="Run Shell script files from Command Prompt" width="600" height="295" srcset="https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Shell-script-files-from-Command-Prompt.png 600w, https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Shell-script-files-from-Command-Prompt-150x74.png 150w, https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Shell-script-files-from-Command-Prompt-400x197.png 400w" sizes="(max-width: 600px) 100vw, 600px" /></noscript></p>
<p>On a Linux platform, you usually use SH, but here you need to use BASH. That said, BASH in Windows has its limitations, so if you want to execute in a Linux environment, you need to install Ubuntu or anything similar.</p><div class="code-block code-block-3" style="margin: 8px 0; clear: both;">
<!-- Ezoic - under_7th_para - under_first_paragraph -->
<span id="ezoic-pub-ad-placeholder-153"></span><span class='ezoic-ad medrectangle-3 medrectangle-3153 adtester-container adtester-container-153' data-ez-name='thewindowsclub_com-medrectangle-3'><span id='div-gpt-ad-thewindowsclub_com-medrectangle-3-0' ezaw='580' ezah='400' style='position:relative;z-index:0;display:inline-block;min-height:400px;min-width:580px;' class='ezoic-ad'><script data-ezscrex='false' data-cfasync='false' type='text/javascript' style='display:none;'>eval(ez_write_tag([[580,400],'thewindowsclub_com-medrectangle-3','ezslot_1',153,'0','0']));</script></span></span>
<!-- End Ezoic - under_7th_para - under_first_paragraph --></div>

<!-- Quick Adsense WordPress Plugin: http://quickadsense.com/ -->
<div class="c24ff8f4a2da697123def04f69833d8b" data-index="1" style="float: none; margin:10px 0 10px 0; text-align:center;">

<!-- Resp TWC/N Post Center -->





</div>

<p><iframe class="lazy lazy-hidden" title="How to run  sh or Shell Script file in Windows 10" width="750" height="422" data-lazy-type="iframe" data-src="https://www.youtube.com/embed/06E5etw4sqk?feature=oembed" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen=""></iframe></p><div class="code-block code-block-4" style="margin: 8px 0; clear: both;">
<!-- Ezoic - under_8th_para - under_first_paragraph -->
<span id="ezoic-pub-ad-placeholder-169"></span>
<!-- End Ezoic - under_8th_para - under_first_paragraph --></div>

<h3>2] Execute Shell Script using Ubuntu on Windows 10</h3>
<p>Make sure you have <a href="https://www.thewindowsclub.com/run-bash-on-windows-10">Ubuntu or any other Linux distros installed</a>.  Ubuntu will mount or make all your Windows directories available under <em>/mnt</em>. So the C drive is available at <em>/mnt/C</em>.  So if the desktop will be available at <em>/mnt/c/users/&lt;username&gt;/desktop</em>.</p>
<p><img loading="lazy" class="lazy lazy-hidden aligncenter size-large wp-image-186224" src="//www.thewindowsclub.com/wp-content/plugins/a3-lazy-load/assets/images/lazy_placeholder.gif" data-lazy-type="image" data-src="https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Script-files-in-Windows-via-Ubuntu-600x187.png" alt="Run Script files in Windows via Ubuntu" width="600" height="187" srcset="" data-srcset="https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Script-files-in-Windows-via-Ubuntu.png 600w, https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Script-files-in-Windows-via-Ubuntu-150x47.png 150w, https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Script-files-in-Windows-via-Ubuntu-400x125.png 400w" sizes="(max-width: 600px) 100vw, 600px"/><noscript><img loading="lazy" class="aligncenter size-large wp-image-186224" src="https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Script-files-in-Windows-via-Ubuntu-600x187.png" alt="Run Script files in Windows via Ubuntu" width="600" height="187" srcset="https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Script-files-in-Windows-via-Ubuntu.png 600w, https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Script-files-in-Windows-via-Ubuntu-150x47.png 150w, https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Script-files-in-Windows-via-Ubuntu-400x125.png 400w" sizes="(max-width: 600px) 100vw, 600px" /></noscript></p>
<p>Now follow these steps</p>
<ol>
<li>Type Bash in run prompt, and it will launch the distro prompt.</li>
<li>Navigate to the folder using “cd” command to the folder where the scripts are available.</li>
<li>Type “sh script.sh” and hit enter.</li>
</ol>
<p>It will execute the script, and if they have a dependency on any of core Linux features.</p><div class="code-block code-block-5" style="margin: 8px 0; clear: both;">
<!-- Ezoic - under_11th_para - under_second_paragraph -->
<span id="ezoic-pub-ad-placeholder-188"></span>
<!-- End Ezoic - under_11th_para - under_second_paragraph --></div>


<!-- Quick Adsense WordPress Plugin: http://quickadsense.com/ -->
<div class="c24ff8f4a2da697123def04f69833d8b" data-index="3" style="float: none; margin:10px 0 10px 0; text-align:center;">
<span style="color: #333399;"><strong><a style="color: #333399;" href="http://www.restoro.com/includes/route.php?tracking=twc&amp;exec=run" target="_blank" rel="nofollow noopener">Download PC Repair Tool to quickly find &amp; fix Windows errors automatically</a></strong></span>
</div>
<p>Since Linux is now available in Windows, you need not use any third party applications like Cygwin. WSL should be enough for most of the scenarios to help you run a shell script in Windows 10.</p><div class="code-block code-block-6" style="margin: 8px 0; clear: both;">
<!-- Ezoic - under_12th_para - under_second_paragraph -->
<span id="ezoic-pub-ad-placeholder-600"></span><span class='ezoic-ad medrectangle-4 medrectangle-4600 adtester-container adtester-container-600' data-ez-name='thewindowsclub_com-medrectangle-4'><span id='div-gpt-ad-thewindowsclub_com-medrectangle-4-0' ezaw='300' ezah='250' style='position:relative;z-index:0;display:inline-block;width:100%;max-width:1200px;margin-left:auto !important;margin-right:auto !important;min-height:250px;min-width:300px;' class='ezoic-ad'><script data-ezscrex='false' data-cfasync='false' type='text/javascript' style='display:none;'>eval(ez_write_tag([[300,250],'thewindowsclub_com-medrectangle-4','ezslot_4',600,'0','0']));</script></span></span>
<!-- End Ezoic - under_12th_para - under_second_paragraph --></div>

<div class="widget_bibblio_recent_posts">		<div id="bib_related-sidebar72105"></div>
		<script>
			var loadRcm = function() {
				Bibblio.initRelatedContent({
					targetElementId: "bib_related-sidebar72105",
					recommendationKey: "854444bf-956a-497f-b5c1-edd8c84e29e3",
					recommendationType: "optimised",
					contentItemId: "b33f8d31-3bd1-43e4-ab01-35294c6db232",
					showRelatedBy: false,
					subtitleField: "description",
					queryStringParams: false,
					styleClasses: "bib--default bib--row-3 bib--font-arial bib--size-18 bib--4by3 bib--spectrum bib__module"
				}, {
					onRecommendationsRendered: function() {
												jQuery("#bib_related-sidebar72105").closest('.widget_bibblio_recent_posts').fadeIn('fast');
											}
				});
			};

			if (window.addEventListener) {
				window.addEventListener('load', loadRcm, false);
			} else if (window.attachEvent) {
				window.attachEvent('onload', loadRcm);
			}
		</script>
		</div>
<!-- Quick Adsense WordPress Plugin: http://quickadsense.com/ -->
<div class="c24ff8f4a2da697123def04f69833d8b" data-index="2" style="float: none; margin:10px 0 10px 0; text-align:center;">
<!-- Ezoic - bottom of page - bottom_of_page -->
<span id="ezoic-pub-ad-placeholder-105"></span><span class='ezoic-ad large-mobile-banner-1 large-mobile-banner-1105 adtester-container adtester-container-105' data-ez-name='thewindowsclub_com-large-mobile-banner-1'><span id='div-gpt-ad-thewindowsclub_com-large-mobile-banner-1-0' ezaw='580' ezah='400' style='position:relative;z-index:0;display:inline-block;min-height:400px;min-width:580px;' class='ezoic-ad'><script data-ezscrex='false' data-cfasync='false' type='text/javascript' style='display:none;'>eval(ez_write_tag([[580,400],'thewindowsclub_com-large-mobile-banner-1','ezslot_5',105,'0','0']));</script></span></span>
<!-- End Ezoic - bottom of page - bottom_of_page -->

</div>

<div style="font-size: 0px; height: 0px; line-height: 0px; margin: 0; padding: 0; clear: both;"></div><img src="//www.thewindowsclub.com/wp-content/plugins/a3-lazy-load/assets/images/lazy_placeholder.gif" data-lazy-type="image" data-src="https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Shell-script-files-from-Command-Prompt.png" class="lazy lazy-hidden ss-hidden-pin-image" alt="Run Shell script files from Command Prompt" data-pin-url="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-pin-media="https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Shell-script-files-from-Command-Prompt.png" data-pin-description="How to run .sh or Shell Script file in Windows 10"/><noscript><img src="https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Shell-script-files-from-Command-Prompt.png" class="ss-hidden-pin-image" alt="Run Shell script files from Command Prompt" data-pin-url="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-pin-media="https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Shell-script-files-from-Command-Prompt.png" data-pin-description="How to run .sh or Shell Script file in Windows 10"/></noscript><!-- AI CONTENT END 1 -->
					
																<ul class="entry-fields">
							
							
							<li><span>Tags:</span> <a href="https://www.thewindowsclub.com/tag/wsl" rel="tag">WSL</a></li>						</ul>
									</div><!-- .Y-Underline-Link -->	
				</div><!-- .entry-content -->

				
				
				<div class="entry-author-box">
	<div class="entry-author-avatar">
		<img alt="AshishMohta@TWC" src="//www.thewindowsclub.com/wp-content/plugins/a3-lazy-load/assets/images/lazy_placeholder.gif" data-lazy-type="image" data-src="https://secure.gravatar.com/avatar/fb6d7213911a177d3cb4af07eac30fdc?s=100&amp;d=avatar_default&amp;r=g" srcset="" data-srcset="https://secure.gravatar.com/avatar/fb6d7213911a177d3cb4af07eac30fdc?s=200&amp;d=avatar_default&amp;r=g 2x" class="lazy lazy-hidden avatar avatar-100 photo" height="100" width="100" itemprop="image" loading="lazy"/><noscript><img alt='AshishMohta@TWC' src='https://secure.gravatar.com/avatar/fb6d7213911a177d3cb4af07eac30fdc?s=100&#038;d=avatar_default&#038;r=g' srcset='https://secure.gravatar.com/avatar/fb6d7213911a177d3cb4af07eac30fdc?s=200&#038;d=avatar_default&#038;r=g 2x' class='avatar avatar-100 photo' height='100' width='100' itemprop="image" loading='lazy'/></noscript>	</div>

	<div class="entry-author-info">
		<p class="entry-author-name">
			
			<a href="https://www.thewindowsclub.com/author/ash5moh8twc">
			    
			    AshishMohta@TWC			</a>
			
		
		</p>

					<div class="entry-author-bio">
				Ashish is a veteran Windows, and Xbox user who excels in writing tips, tricks, and features on it to improve your day to day experience with your devices.			</div>
		
		
	</div>
<span id="ezoic-pub-ad-placeholder-878" class="ezoic-adpicker-ad"></span></div>

				
				<div id="disqus_thread">
		</div>

			
		</div><!-- .col-md-8 .col-sm-12 .col-xs-12 -->

		<div class="col-md-4 col-sm-12 col-xs-12">
			<div class="sidebar">
	<aside id="text-422067542" class="widget group widget_text">			<div class="textwidget"><table class=" aligncenter" style="border-collapse: collapse; width: 196px; height: 33px;">
<tbody>
<tr>
<td style="padding-right: 4px;"><a href="https://www.facebook.com/TheWindowsClub/" target="_blank" rel="nofollow noopener"><img loading="lazy" class="alignnone wp-image-226453 size-full" src="https://www.thewindowsclub.com/wp-content/uploads/2020/08/icon-fb.png" alt="icon-fb" width="32" height="32"/></a></td>
<td style="padding-right: 4px;"><a href="https://twitter.com/TheWindowsClub" target="_blank" rel="nofollow noopener"><img loading="lazy" class="alignnone wp-image-226452 size-full" src="https://www.thewindowsclub.com/wp-content/uploads/2020/08/icon-twitter.png" alt="icon-twitter" width="32" height="32"/></a></td>
<td style="padding-right: 4px;"><a href="http://feeds.feedburner.com/TheWindowsClub" target="_blank" rel="nofollow noopener"><img loading="lazy" class="alignnone wp-image-226451 size-full" src="https://www.thewindowsclub.com/wp-content/uploads/2020/08/rss-icon_32.png" alt="rss-icon_32" width="32" height="32"/></a></td>
<td style="padding-right: 4px;"><a href="https://www.youtube.com/c/TheWindowsClubVideos?sub_confirmation=1" target="_blank" rel="nofollow noopener"><img loading="lazy" class="alignnone wp-image-226454 size-full" src="https://www.thewindowsclub.com/wp-content/uploads/2020/08/youtube-icon_32.png" alt="icon-yt" width="32" height="32"/></a></td>
<td style="padding-right: 4px;"><a href="https://feedburner.google.com/fb/a/mailverify?uri=TheWindowsClub" target="_blank" rel="nofollow noopener"><img loading="lazy" class="alignnone wp-image-226450 size-full" src="https://www.thewindowsclub.com/wp-content/uploads/2020/08/eMail-icon_32.png" alt="eMail-icon_32" width="32" height="32"/></a></td>
<td style="padding-right: 4px;"><a href="https://www.thewindowsclub.com/connect-windows-club" target="_blank" rel="noopener"><img loading="lazy" class="alignnone wp-image-226449 size-full" src="https://www.thewindowsclub.com/wp-content/uploads/2020/08/connect-icon-1.png" alt="connect-icon-1" width="32" height="32"/></a></td>
</tr>
</tbody>
</table>
</div>
		</aside><aside id="text-422067543" class="widget group widget_text">			<div class="textwidget"><p><!-- Ezoic - sidebar 870 - sidebar --></p>
<span id="ezoic-pub-ad-placeholder-870"></span><span class='ezoic-ad box-1 box-1870 adtester-container adtester-container-870' data-ez-name='thewindowsclub_com-box-1'><span id='div-gpt-ad-thewindowsclub_com-box-1-0' ezaw='336' ezah='280' style='position:relative;z-index:0;display:inline-block;min-height:280px;min-width:336px;' class='ezoic-ad'><script data-ezscrex='false' data-cfasync='false' type='text/javascript' style='display:none;'>eval(ez_write_tag([[336,280],'thewindowsclub_com-box-1','ezslot_3',870,'0','0']));</script></span><span style='width:336px;display:block;height:14px;margin:auto' class='reportline'><span style='text-align:center;font-size: smaller;float:left;line-height:normal;'><a href='https://www.ezoic.com/what-is-ezoic/' target='_blank' rel='noopener noreferrer nofollow' style='cursor:pointer'/><img src='https://go.ezoic.net/utilcave_com/img/ezoic.png' alt="Ezoic" style='height:12px !important; padding:2px !important; border:0px !important; cursor:pointer !important; width: 58px !important; margin:0 !important; box-sizing: content-box !important;'/></a></span><span class='ez-report-ad-button' name='?pageview_id=c2eeeada-291f-4952-4ff1-a0e3639cb84d&ad_position_id=870&impression_group_id=thewindowsclub_com-box-1/2021-03-04/1442631&ad_size=336x280&domain_id=77472&url=https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10' style='cursor: pointer!important; font-size:12px !important;color: #a5a5a5 ;float:right;text-decoration:none !important;font-family:arial !important;line-height:normal;'>report this ad</span></span></span>
<p><!-- End Ezoic - sidebar 870 - sidebar --></p>
</div>
		</aside><aside id="text-422067551" class="widget group widget_text">			<div class="textwidget"><p><script src="https://player.anyclip.com/anyclip-widget/lre-widget/prod/v1/src/lre.js" pubname="thewindowsclubcom" widgetname="0011r00002JOYIf_932">
</script></p>
</div>
		</aside><aside id="feedzy_wp_widget-3" class="widget group widget_feedzy_wp_widget"><h3 class="widget-title">Latest News</h3><div class="feedzy-lazy" data-feeds="https://news.thewindowsclub.com/feed/" data-max="2" data-feed_title="no" data-target="_blank" data-follow="" data-title="" data-meta="no" data-multiple_meta="" data-summary="no" data-summarylength="70" data-thumb="auto" data-default="" data-size="" data-keywords_title="" data-keywords_inc="" data-refresh="3_hours" data-sort="date_desc" data-http="" data-error_empty="" data-amp="yes" data-offset="" data-classname="" data-lazy="yes" data-_dryrun_="no" data-_dry_run_tags_="" data-price="no" data-referral_url="" data-keywords_ban="" data-columns="1" data-template="style2" data-mapping=""><div class="feedzy-rss ">
		<ul class="feedzy-style2">
					<li style="padding: 15px 0 25px" class="rss_item feedzy-rss-col-1">
									<div class="rss_image" style="width:150px; height:150px;">
						<a href="https://news.thewindowsclub.com/intel-releases-new-drivers-with-fixes-for-windows-10-105214/" target="_blank" rel="noopener " title="Intel releases new Drivers with fixes for Windows 10" style="width:150px; height:150px;">
							<span class="fetched" style="background-image:  url(&#39;https://news.thewindowsclub.com/wp-content/uploads/2020/09/Intel-logo-2020-300x127.jpg&#39;);" title="Intel releases new Drivers with fixes for Windows 10"></span><amp-img width="150" height="150" src="https://news.thewindowsclub.com/wp-content/uploads/2020/09/Intel-logo-2020-300x127.jpg">						</amp-img></a>
					</div>
								<div class="rss_content_wrap">
					<span class="title">
						<a href="https://news.thewindowsclub.com/intel-releases-new-drivers-with-fixes-for-windows-10-105214/" target="_blank" rel="noopener ">
							Intel releases new Drivers with fixes for Windows 10						</a>
					</span>
					<div class="rss_content" style="">
						<small class="meta"></small>

						<p class="description"></p>

						
											</div>
				</div>
			</li>
						<li style="padding: 15px 0 25px" class="rss_item feedzy-rss-col-1">
									<div class="rss_image" style="width:150px; height:150px;">
						<a href="https://news.thewindowsclub.com/microsoft-digital-marketing-center-105208/" target="_blank" rel="noopener " title="Microsoft lets you create a free Website via Digital Marketing Center" style="width:150px; height:150px;">
							<span class="fetched" style="background-image:  url(&#39;https://news.thewindowsclub.com/wp-content/uploads/2021/02/Create-Free-Website-Digital-Marketing-Center-300x202.jpg&#39;);" title="Microsoft lets you create a free Website via Digital Marketing Center"></span><amp-img width="150" height="150" src="https://news.thewindowsclub.com/wp-content/uploads/2021/02/Create-Free-Website-Digital-Marketing-Center-300x202.jpg">						</amp-img></a>
					</div>
								<div class="rss_content_wrap">
					<span class="title">
						<a href="https://news.thewindowsclub.com/microsoft-digital-marketing-center-105208/" target="_blank" rel="noopener ">
							Microsoft lets you create a free Website via Digital Marketing Center						</a>
					</span>
					<div class="rss_content" style="">
						<small class="meta"></small>

						<p class="description"></p>

						
											</div>
				</div>
			</li>
				</ul>
</div>
</div></aside><aside id="feedzy_wp_widget-2" class="widget group widget_feedzy_wp_widget"><h3 class="widget-title">Latest Reviews</h3><div class="feedzy-lazy" data-feeds="https://reviews.thewindowsclub.com/feed/" data-max="2" data-feed_title="no" data-target="_blank" data-follow="" data-title="" data-meta="no" data-multiple_meta="" data-summary="no" data-summarylength="70" data-thumb="auto" data-default="" data-size="" data-keywords_title="" data-keywords_inc="" data-refresh="12_hours" data-sort="date_desc" data-http="" data-error_empty="" data-amp="yes" data-offset="" data-classname="" data-lazy="yes" data-_dryrun_="no" data-_dry_run_tags_="" data-price="no" data-referral_url="" data-keywords_ban="" data-columns="1" data-template="style2" data-mapping=""><div class="feedzy-rss ">
		<ul class="feedzy-style2">
					<li style="padding: 15px 0 25px" class="rss_item feedzy-rss-col-1">
									<div class="rss_image" style="width:150px; height:150px;">
						<a href="https://reviews.thewindowsclub.com/best-ways-to-make-great-marketing-videos/" target="_blank" rel="noopener " title="5 Best Ways To Make Great Marketing Videos" style="width:150px; height:150px;">
							<span class="fetched" style="background-image:  url(&#39;https://reviews.thewindowsclub.com/wp-content/uploads/2021/01/How-To-Make-Great-Marketing-Videos.jpg&#39;);" title="5 Best Ways To Make Great Marketing Videos"></span><amp-img width="150" height="150" src="https://reviews.thewindowsclub.com/wp-content/uploads/2021/01/How-To-Make-Great-Marketing-Videos.jpg">						</amp-img></a>
					</div>
								<div class="rss_content_wrap">
					<span class="title">
						<a href="https://reviews.thewindowsclub.com/best-ways-to-make-great-marketing-videos/" target="_blank" rel="noopener ">
							5 Best Ways To Make Great Marketing Videos						</a>
					</span>
					<div class="rss_content" style="">
						<small class="meta"></small>

						<p class="description"></p>

						
											</div>
				</div>
			</li>
						<li style="padding: 15px 0 25px" class="rss_item feedzy-rss-col-1">
									<div class="rss_image" style="width:150px; height:150px;">
						<a href="https://reviews.thewindowsclub.com/flexclip-review-video-marketing/" target="_blank" rel="noopener " title="FlexClip Review: All in one Video Maker for your Daily Video Marketing" style="width:150px; height:150px;">
							<span class="fetched" style="background-image:  url(&#39;https://reviews.thewindowsclub.com/wp-content/uploads/2021/02/FlexClip-homepage.png&#39;);" title="FlexClip Review: All in one Video Maker for your Daily Video Marketing"></span><amp-img width="150" height="150" src="https://reviews.thewindowsclub.com/wp-content/uploads/2021/02/FlexClip-homepage.png">						</amp-img></a>
					</div>
								<div class="rss_content_wrap">
					<span class="title">
						<a href="https://reviews.thewindowsclub.com/flexclip-review-video-marketing/" target="_blank" rel="noopener ">
							FlexClip Review: All in one Video Maker for your Daily Video Marketing						</a>
					</span>
					<div class="rss_content" style="">
						<small class="meta"></small>

						<p class="description"></p>

						
											</div>
				</div>
			</li>
				</ul>
</div>
</div></aside><aside id="text-422067541" class="widget group widget_text">			<div class="textwidget"><p></p><center><!-- Ezoic - sidebar floating - sidebar_floating_1 --></center><p></p>
<span id="ezoic-pub-ad-placeholder-104"></span><span class='ezoic-ad banner-2 banner-2104 adtester-container adtester-container-104' data-ez-name='thewindowsclub_com-banner-2'><span id='div-gpt-ad-thewindowsclub_com-banner-2-0' ezaw='300' ezah='600' style='position:relative;z-index:0;display:inline-block;min-height:600px;min-width:300px;' class='ezoic-ad'><script data-ezscrex='false' data-cfasync='false' type='text/javascript' style='display:none;'>eval(ez_write_tag([[300,600],'thewindowsclub_com-banner-2','ezslot_2',104,'0','0']));</script></span><span style='width:300px;display:block;height:14px;margin:auto' class='reportline'><span style='text-align:center;font-size: smaller;float:left;line-height:normal;'><a href='https://www.ezoic.com/what-is-ezoic/' target='_blank' rel='noopener noreferrer nofollow' style='cursor:pointer'/><img src='https://go.ezoic.net/utilcave_com/img/ezoic.png' alt="Ezoic" style='height:12px !important; padding:2px !important; border:0px !important; cursor:pointer !important; width: 58px !important; margin:0 !important; box-sizing: content-box !important;'/></a></span><span class='ez-report-ad-button' name='?pageview_id=c2eeeada-291f-4952-4ff1-a0e3639cb84d&ad_position_id=104&impression_group_id=thewindowsclub_com-banner-2/2021-03-04/1495879&ad_size=300x600&domain_id=77472&url=https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10' style='cursor: pointer!important; font-size:12px !important;color: #a5a5a5 ;float:right;text-decoration:none !important;font-family:arial !important;line-height:normal;'>report this ad</span></span></span>
<p><!-- End Ezoic - sidebar floating - sidebar_floating_1 --></p>
</div>
		</aside></div>
		</div>
	</div><!-- .row -->

</div><!-- .col-xs-12 -->

		</div>
	</div>
</main>

<footer class="footer">
	<div class="container"><span id="ezoic-pub-ad-placeholder-121" class="ezoic-adpicker-ad"></span><span class='ezoic-ad medrectangle-1 medrectangle-1121 adtester-container adtester-container-121' data-ez-name='thewindowsclub_com-medrectangle-1'><span id='div-gpt-ad-thewindowsclub_com-medrectangle-1-0' ezaw='728' ezah='90' style='position:relative;z-index:0;display:inline-block;min-height:90px;min-width:728px;' class='ezoic-ad'><script data-ezscrex='false' data-cfasync='false' type='text/javascript' style='display:none;'>eval(ez_write_tag([[728,90],'thewindowsclub_com-medrectangle-1','ezslot_6',121,'0','0']));</script></span><span style='width:728px;display:block;height:14px;margin:auto' class='reportline'><span style='text-align:center;font-size: smaller;float:left;line-height:normal;'><a href='https://www.ezoic.com/what-is-ezoic/' target='_blank' rel='noopener noreferrer nofollow' style='cursor:pointer'/><img src='https://go.ezoic.net/utilcave_com/img/ezoic.png' alt="Ezoic" style='height:12px !important; padding:2px !important; border:0px !important; cursor:pointer !important; width: 58px !important; margin:0 !important; box-sizing: content-box !important;'/></a></span><span class='ez-report-ad-button' name='?pageview_id=c2eeeada-291f-4952-4ff1-a0e3639cb84d&ad_position_id=121&impression_group_id=thewindowsclub_com-medrectangle-1/2021-03-04/1471876&ad_size=728x90&domain_id=77472&url=https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10' style='cursor: pointer!important; font-size:12px !important;color: #a5a5a5 ;float:right;text-decoration:none !important;font-family:arial !important;line-height:normal;'>report this ad</span></span></span>
		<div class="row">
			<div class="col-sm-4">
				<aside id="text-422067545" class="widget group widget_text">			<div class="textwidget"><div class="mobileHide"><br/>
<!-- Async 970x90 Large Horizontal TWC/N --><br/>
</div>
</div>
		</aside>			</div>

			<div class="col-sm-4">
							</div>

			<div class="col-sm-4">
							</div>
		</div>
	</div>

	<div class="foot">
		<div class="container">
			<div class="row">
				<div class="col-xs-12">
					<p>
											</p>

				</div>
			</div>
		</div>
	</div>
</footer>

</div> <!-- #page -->

<!-- Global site tag (gtag.js) - Google Analytics -->
<script async="" src="https://www.googletagmanager.com/gtag/js?id=UA-8662655-1"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'UA-8662655-1');
</script>

<!-- Admiral Visitor Relationship Management Tag for thewindowsclub.com -->
<script type="text/javascript">!(function(o,n,t){t=o.createElement(n),o=o.getElementsByTagName(n)[0],t.async=1,t.src="https://stormyachiever.com/v2imy4XN5DQoCzfgoNvjynTCn0bdm19qW5-w0Hpbky-AI6hLQiNcl7IXQJ7ASXlJWZS4KMj8poAtp9fj5KEQzYCq8ZMoqRyE",o.parentNode.insertBefore(t,o)})(document,"script"),(function(o,n){o[n]=o[n]||function(){(o[n].q=o[n].q||[]).push(arguments)}})(window,"admiral");!(function(c,e,o,t,n){function r(o,t){(function n(){try{return 0<(localStorage.getItem("v4ac1eiZr0")||"").split(",")[4]}catch(o){}return!1})()&&(t=c[e].pubads())&&t.setTargeting("admiral-engaged","true")}(n=c[e]=c[e]||{}).cmd=n.cmd||[],typeof n.pubads===o?r():typeof n.cmd.unshift===o?n.cmd.unshift(r):n.cmd.push(r)})(window,"googletag","function");</script>		<div id="ss-floating-bar" class="ss-entrance-animation-slide ss-animate-entrance ss-hover-animation-1 ss-hover-animation-2 ss-left-sidebar ss-small-icons ss-hide-on-mobile ss-circle-icons" data-offset="-20">

			
		<span class="ss-total-counter ss-total-shares ss-share-sidebar-total-shares" data-ss-ss-post-id="186120">
			<span>79</span>
			<span>Shares</span>
		</span>

		
		<ul class="ss-social-icons-container">

							<li class="">

					
						
						<a href="#" data-ss-ss-link="https://www.facebook.com/sharer.php?t=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010&amp;u=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10" class="ss-facebook-color" rel="nofollow noopener" data-ss-ss-network-id="facebook" data-ss-ss-post-id="186120" data-ss-ss-location="sidebar" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" data-has-api="true">
					
						<span class="ss-share-network-content">
							<i class="ss-network-icon"><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M32 16.098C32 7.208 24.837 0 16 0S0 7.207 0 16.098C0 24.133 5.851 30.792 13.5 32V20.751H9.437v-4.653H13.5V12.55c0-4.034 2.389-6.263 6.043-6.263 1.751 0 3.582.315 3.582.315v3.961h-2.018c-1.987 0-2.607 1.241-2.607 2.514v3.02h4.438l-.71 4.653H18.5V32C26.149 30.792 32 24.133 32 16.098z"></path></svg></i>

															<i class="ss-network-icon ss-slide-icon"><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M32 16.098C32 7.208 24.837 0 16 0S0 7.207 0 16.098C0 24.133 5.851 30.792 13.5 32V20.751H9.437v-4.653H13.5V12.55c0-4.034 2.389-6.263 6.043-6.263 1.751 0 3.582.315 3.582.315v3.961h-2.018c-1.987 0-2.607 1.241-2.607 2.514v3.02h4.438l-.71 4.653H18.5V32C26.149 30.792 32 24.133 32 16.098z"></path></svg></i>
								
							
						</span>

											</a>
					
									</li>
							<li class="">

					
						
						<a href="#" data-ss-ss-link="https://twitter.com/intent/tweet?text=How+to+run+.sh+or+Shell+Script+file+in+Windows+10&amp;url=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10" class="ss-twitter-color" rel="nofollow noopener" data-ss-ss-network-id="twitter" data-ss-ss-post-id="186120" data-ss-ss-location="sidebar" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share">
					
						<span class="ss-share-network-content">
							<i class="ss-network-icon"><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M28.75 9.5c0 0.25 0 0.563 0 0.813 0 8.688-6.625 18.688-18.688 18.688-3.688 0-7.188-1.063-10.063-2.938 0.5 0.063 1.063 0.063 1.563 0.063 3.063 0 5.938-1 8.188-2.813-2.875 0-5.313-1.938-6.188-4.563 0.438 0.125 0.813 0.125 1.25 0.125 0.625 0 1.188-0.063 1.75-0.188-3-0.625-5.25-3.313-5.25-6.438 0-0.063 0-0.063 0-0.125 0.875 0.5 1.875 0.813 2.938 0.813-1.75-1.125-2.938-3.188-2.938-5.438 0-1.188 0.375-2.313 0.938-3.313 3.188 4 8.063 6.625 13.5 6.875-0.125-0.5-0.188-1-0.188-1.5 0-3.625 2.938-6.563 6.563-6.563 1.938 0 3.625 0.813 4.813 2.063 1.5-0.313 2.938-0.813 4.188-1.563-0.5 1.5-1.563 2.813-2.875 3.625 1.313-0.188 2.563-0.5 3.75-1.063-0.875 1.313-2 2.5-3.25 3.438z"></path></svg></i>

															<i class="ss-network-icon ss-slide-icon"><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M28.75 9.5c0 0.25 0 0.563 0 0.813 0 8.688-6.625 18.688-18.688 18.688-3.688 0-7.188-1.063-10.063-2.938 0.5 0.063 1.063 0.063 1.563 0.063 3.063 0 5.938-1 8.188-2.813-2.875 0-5.313-1.938-6.188-4.563 0.438 0.125 0.813 0.125 1.25 0.125 0.625 0 1.188-0.063 1.75-0.188-3-0.625-5.25-3.313-5.25-6.438 0-0.063 0-0.063 0-0.125 0.875 0.5 1.875 0.813 2.938 0.813-1.75-1.125-2.938-3.188-2.938-5.438 0-1.188 0.375-2.313 0.938-3.313 3.188 4 8.063 6.625 13.5 6.875-0.125-0.5-0.188-1-0.188-1.5 0-3.625 2.938-6.563 6.563-6.563 1.938 0 3.625 0.813 4.813 2.063 1.5-0.313 2.938-0.813 4.188-1.563-0.5 1.5-1.563 2.813-2.875 3.625 1.313-0.188 2.563-0.5 3.75-1.063-0.875 1.313-2 2.5-3.25 3.438z"></path></svg></i>
								
							
						</span>

											</a>
					
									</li>
							<li class="ss-hide-on-mobile">

					
						
						<a href="#" data-ss-ss-link="https://www.linkedin.com/shareArticle?title=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010&amp;url=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10&amp;mini=true" class="ss-linkedin-color" rel="nofollow noopener" data-ss-ss-network-id="linkedin" data-ss-ss-post-id="186120" data-ss-ss-location="sidebar" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share">
					
						<span class="ss-share-network-content">
							<i class="ss-network-icon"><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M29.632 0C30.939 0 32 1.032 32 2.307v27.384C32 30.966 30.939 32 29.632 32H2.36C1.058 32 0 30.966 0 29.69V2.308C0 1.032 1.058 0 2.36 0h27.272zM9.149 11.638h-4.77V27h4.77V11.638zm12.133-.382c-2.318 0-3.874 1.273-4.509 2.48h-.066v-2.098H12.14V27h4.76v-7.599c0-2.004.378-3.946 2.858-3.946 2.447 0 2.475 2.29 2.475 4.072V27H27v-8.423c0-4.138-.893-7.32-5.718-7.32v-.001zM6.764 4A2.766 2.766 0 004 6.769a2.765 2.765 0 105.528 0A2.767 2.767 0 006.765 4h-.001z"></path></svg></i>

															<i class="ss-network-icon ss-slide-icon"><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M29.632 0C30.939 0 32 1.032 32 2.307v27.384C32 30.966 30.939 32 29.632 32H2.36C1.058 32 0 30.966 0 29.69V2.308C0 1.032 1.058 0 2.36 0h27.272zM9.149 11.638h-4.77V27h4.77V11.638zm12.133-.382c-2.318 0-3.874 1.273-4.509 2.48h-.066v-2.098H12.14V27h4.76v-7.599c0-2.004.378-3.946 2.858-3.946 2.447 0 2.475 2.29 2.475 4.072V27H27v-8.423c0-4.138-.893-7.32-5.718-7.32v-.001zM6.764 4A2.766 2.766 0 004 6.769a2.765 2.765 0 105.528 0A2.767 2.767 0 006.765 4h-.001z"></path></svg></i>
								
							
						</span>

											</a>
					
									</li>
							<li class="ss-hide-on-mobile">

					
						
						<a href="#" data-ss-ss-link="https://www.reddit.com/submit?title=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010&amp;url=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10" class="ss-reddit-color" rel="nofollow noopener" data-ss-ss-network-id="reddit" data-ss-ss-post-id="186120" data-ss-ss-location="sidebar" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share">
					
						<span class="ss-share-network-content">
							<i class="ss-network-icon"><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M32 15.75c0-1.75-1.375-3.125-3.125-3.125-1 0-1.875 0.438-2.438 1.188-2.5-1.813-6-2.938-9.938-3l2.313-6.875 5.75 1.375c0.125 0 0.188 0 0.25 0 0.063 1.313 1.125 2.375 2.5 2.375s2.438-1.125 2.438-2.5c0-1.375-1.063-2.438-2.438-2.438-1.063 0-1.875 0.563-2.313 1.438 0 0-0.063-0.063-0.125-0.063l-6.313-1.5c-0.313-0.063-0.625 0.125-0.688 0.375l-2.688 7.813c-3.813 0.125-7.188 1.188-9.688 2.938-0.563-0.688-1.375-1.125-2.375-1.125-1.75 0-3.125 1.375-3.125 3.125 0 1.25 0.75 2.375 1.875 2.875-0.125 0.438-0.188 0.938-0.188 1.438 0 5.125 6.375 9.313 14.25 9.313s14.25-4.188 14.25-9.313c0-0.438-0.063-0.938-0.188-1.375 1.188-0.5 2-1.625 2-2.938zM8.688 18.25c0-1.25 1.063-2.313 2.313-2.313s2.313 1.063 2.313 2.313c0 1.25-1.063 2.313-2.313 2.313s-2.313-1.063-2.313-2.313zM21.188 24.625c-1.063 1.063-2.75 1.563-5.188 1.563s-4.125-0.5-5.188-1.563c-0.125-0.125-0.125-0.375 0-0.563 0.125-0.125 0.375-0.125 0.5 0 0.938 0.938 2.438 1.375 4.688 1.375 2.188 0 3.75-0.438 4.688-1.375 0.125-0.125 0.375-0.125 0.5 0 0.125 0.188 0.125 0.438 0 0.563zM21.063 20.563c-1.313 0-2.375-1-2.375-2.313 0-1.25 1.063-2.313 2.375-2.313 1.25 0 2.25 1.063 2.25 2.313 0 1.313-1 2.313-2.25 2.313z"></path></svg></i>

															<i class="ss-network-icon ss-slide-icon"><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M32 15.75c0-1.75-1.375-3.125-3.125-3.125-1 0-1.875 0.438-2.438 1.188-2.5-1.813-6-2.938-9.938-3l2.313-6.875 5.75 1.375c0.125 0 0.188 0 0.25 0 0.063 1.313 1.125 2.375 2.5 2.375s2.438-1.125 2.438-2.5c0-1.375-1.063-2.438-2.438-2.438-1.063 0-1.875 0.563-2.313 1.438 0 0-0.063-0.063-0.125-0.063l-6.313-1.5c-0.313-0.063-0.625 0.125-0.688 0.375l-2.688 7.813c-3.813 0.125-7.188 1.188-9.688 2.938-0.563-0.688-1.375-1.125-2.375-1.125-1.75 0-3.125 1.375-3.125 3.125 0 1.25 0.75 2.375 1.875 2.875-0.125 0.438-0.188 0.938-0.188 1.438 0 5.125 6.375 9.313 14.25 9.313s14.25-4.188 14.25-9.313c0-0.438-0.063-0.938-0.188-1.375 1.188-0.5 2-1.625 2-2.938zM8.688 18.25c0-1.25 1.063-2.313 2.313-2.313s2.313 1.063 2.313 2.313c0 1.25-1.063 2.313-2.313 2.313s-2.313-1.063-2.313-2.313zM21.188 24.625c-1.063 1.063-2.75 1.563-5.188 1.563s-4.125-0.5-5.188-1.563c-0.125-0.125-0.125-0.375 0-0.563 0.125-0.125 0.375-0.125 0.5 0 0.938 0.938 2.438 1.375 4.688 1.375 2.188 0 3.75-0.438 4.688-1.375 0.125-0.125 0.375-0.125 0.5 0 0.125 0.188 0.125 0.438 0 0.563zM21.063 20.563c-1.313 0-2.375-1-2.375-2.313 0-1.25 1.063-2.313 2.375-2.313 1.25 0 2.25 1.063 2.25 2.313 0 1.313-1 2.313-2.25 2.313z"></path></svg></i>
								
							
						</span>

											</a>
					
									</li>
							<li class="ss-hide-on-desktop">

					
						
						<a href="#" data-ss-ss-link="https://api.whatsapp.com/send?text=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010%20https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10" class="ss-whatsapp-color" rel="nofollow noopener" data-ss-ss-network-id="whatsapp" data-ss-ss-post-id="186120" data-ss-ss-location="sidebar" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share">
					
						<span class="ss-share-network-content">
							<i class="ss-network-icon"><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M27.313 4.625c-3-3-7-4.625-11.25-4.625-8.75 0-15.875 7.125-15.875 15.875 0 2.75 0.75 5.5 2.125 7.938l-2.25 8.188 8.438-2.188c2.313 1.25 4.875 1.938 7.563 1.938v0c0 0 0 0 0 0 8.75 0 15.875-7.125 15.875-15.875 0-4.25-1.625-8.25-4.625-11.25zM16.063 29.063v0c-2.375 0-4.688-0.625-6.688-1.875l-0.5-0.25-5 1.313 1.313-4.875-0.313-0.5c-1.313-2.125-2-4.5-2-7 0-7.313 5.938-13.188 13.188-13.188 3.5 0 6.813 1.375 9.313 3.875s3.875 5.813 3.875 9.313c0 7.25-5.938 13.188-13.188 13.188zM23.313 19.188c-0.438-0.188-2.375-1.188-2.75-1.313-0.313-0.125-0.625-0.188-0.875 0.188-0.25 0.438-1 1.313-1.25 1.563s-0.438 0.313-0.875 0.125c-0.375-0.188-1.625-0.625-3.188-2-1.125-1-1.938-2.313-2.188-2.75-0.25-0.375 0-0.563 0.188-0.813 0.188-0.125 0.375-0.438 0.563-0.688 0.25-0.188 0.313-0.375 0.438-0.625s0.063-0.5-0.063-0.688c-0.063-0.188-0.875-2.188-1.188-2.938-0.375-0.813-0.688-0.688-0.938-0.688-0.188 0-0.5 0-0.75 0s-0.688 0.063-1.063 0.438c-0.375 0.438-1.375 1.375-1.375 3.313 0 2 1.438 3.875 1.625 4.125s2.813 4.25 6.75 6c0.938 0.375 1.688 0.625 2.25 0.813 1 0.313 1.813 0.25 2.5 0.188 0.813-0.125 2.375-1 2.688-1.938 0.375-0.875 0.375-1.688 0.25-1.875-0.125-0.125-0.375-0.25-0.75-0.438z"></path></svg></i>

															<i class="ss-network-icon ss-slide-icon"><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M27.313 4.625c-3-3-7-4.625-11.25-4.625-8.75 0-15.875 7.125-15.875 15.875 0 2.75 0.75 5.5 2.125 7.938l-2.25 8.188 8.438-2.188c2.313 1.25 4.875 1.938 7.563 1.938v0c0 0 0 0 0 0 8.75 0 15.875-7.125 15.875-15.875 0-4.25-1.625-8.25-4.625-11.25zM16.063 29.063v0c-2.375 0-4.688-0.625-6.688-1.875l-0.5-0.25-5 1.313 1.313-4.875-0.313-0.5c-1.313-2.125-2-4.5-2-7 0-7.313 5.938-13.188 13.188-13.188 3.5 0 6.813 1.375 9.313 3.875s3.875 5.813 3.875 9.313c0 7.25-5.938 13.188-13.188 13.188zM23.313 19.188c-0.438-0.188-2.375-1.188-2.75-1.313-0.313-0.125-0.625-0.188-0.875 0.188-0.25 0.438-1 1.313-1.25 1.563s-0.438 0.313-0.875 0.125c-0.375-0.188-1.625-0.625-3.188-2-1.125-1-1.938-2.313-2.188-2.75-0.25-0.375 0-0.563 0.188-0.813 0.188-0.125 0.375-0.438 0.563-0.688 0.25-0.188 0.313-0.375 0.438-0.625s0.063-0.5-0.063-0.688c-0.063-0.188-0.875-2.188-1.188-2.938-0.375-0.813-0.688-0.688-0.938-0.688-0.188 0-0.5 0-0.75 0s-0.688 0.063-1.063 0.438c-0.375 0.438-1.375 1.375-1.375 3.313 0 2 1.438 3.875 1.625 4.125s2.813 4.25 6.75 6c0.938 0.375 1.688 0.625 2.25 0.813 1 0.313 1.813 0.25 2.5 0.188 0.813-0.125 2.375-1 2.688-1.938 0.375-0.875 0.375-1.688 0.25-1.875-0.125-0.125-0.375-0.25-0.75-0.438z"></path></svg></i>
								
							
						</span>

											</a>
					
									</li>
			
			
				<li>
					<a href="#" class="ss-share-all ss-shareall-color" rel="nofollow noopener">
						<span class="ss-share-network-content">
							<i class="ss-network-icon"><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M25.333 15.333h-8v-8c0-0.733-0.6-1.333-1.333-1.333s-1.333 0.6-1.333 1.333v8h-8c-0.733 0-1.333 0.6-1.333 1.333s0.6 1.333 1.333 1.333h8v8c0 0.733 0.6 1.333 1.333 1.333s1.333-0.6 1.333-1.333v-8h8c0.733 0 1.333-0.6 1.333-1.333s-0.6-1.333-1.333-1.333z"></path></svg></i>

														<i class="ss-network-icon ss-slide-icon"><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M25.333 15.333h-8v-8c0-0.733-0.6-1.333-1.333-1.333s-1.333 0.6-1.333 1.333v8h-8c-0.733 0-1.333 0.6-1.333 1.333s0.6 1.333 1.333 1.333h8v8c0 0.733 0.6 1.333 1.333 1.333s1.333-0.6 1.333-1.333v-8h8c0.733 0 1.333-0.6 1.333-1.333s-0.6-1.333-1.333-1.333z"></path></svg></i>
														</span>
					</a>

					
				</li>
					</ul>
		
			<span class="ss-hide-floating-bar">
				<svg xmlns="http://www.w3.org/2000/svg" width="13" height="13" viewBox="0 0 370.814 370.814"><path d="M292.92 24.848L268.781 0 77.895 185.401l190.886 185.413 24.139-24.853-165.282-160.56"></path></svg>
			</span>

		</div><!-- END #ss-floating-bar -->
		<link rel="stylesheet" id="feedzy-rss-feeds-css" href="https://www.thewindowsclub.com/wp-content/plugins/feedzy-rss-feeds/css/feedzy-rss-feeds.css?ver=3.5.2" type="text/css" media="all"/>
<script type="text/javascript" src="//cdn.bibblio.org/rcm/4.6/bib-related-content.js?ver=5.6.2" id="bibblio-rcm-js-js"></script>
<script type="text/javascript" id="dcl_comments-js-extra">
/* <![CDATA[ */
var countVars = {"disqusShortname":"thewindowsclub"};
var embedVars = {"disqusConfig":{"integration":"wordpress 3.0.16"},"disqusIdentifier":"186120 https:\/\/www.thewindowsclub.com\/?p=186120","disqusShortname":"thewindowsclub","disqusTitle":"How to run .sh or Shell Script file in Windows 10","disqusUrl":"https:\/\/www.thewindowsclub.com\/how-to-run-sh-or-shell-script-file-in-windows-10","postId":"186120"};
var dclCustomVars = {"dcl_progress_text":"Loading comments..."};
/* ]]> */
</script>
<script type="text/javascript" src="https://www.thewindowsclub.com/wp-content/plugins/disqus-conditional-load/assets/js/public/embed-scroll.min.js?ver=11.0.5" id="dcl_comments-js"></script>
<script type="text/javascript" id="socialsnap-js-js-extra">
/* <![CDATA[ */
var socialsnap_script = {"ajaxurl":"https:\/\/www.thewindowsclub.com\/wp-admin\/admin-ajax.php","on_media_width":"250","on_media_height":"250","nonce":"6f921c909c","post_id":"186120","click_tracking":""};
/* ]]> */
</script>
<script type="text/javascript" src="https://www.thewindowsclub.com/wp-content/plugins/socialsnap-pro/assets/js/socialsnap.js?ver=1.1.15" id="socialsnap-js-js"></script>
<script type="text/javascript" src="https://www.thewindowsclub.com/wp-content/themes/noozbeat/js/superfish.js?ver=1.7.5" id="superfish-js"></script>
<script type="text/javascript" src="https://www.thewindowsclub.com/wp-content/themes/noozbeat/js/jquery.mmenu.min.all.js?ver=5.2.0" id="mmenu-js"></script>
<script type="text/javascript" src="https://www.thewindowsclub.com/wp-content/themes/noozbeat/js/jquery.flexslider.js?ver=2.5.0" id="flexslider-js"></script>
<script type="text/javascript" src="https://www.thewindowsclub.com/wp-content/themes/noozbeat/js/jquery.fitvids.js?ver=1.1" id="fitVids-js"></script>
<script type="text/javascript" src="https://www.thewindowsclub.com/wp-content/themes/noozbeat/js/jquery.magnific-popup.js?ver=1.0.0" id="magnific-popup-js"></script>
<script type="text/javascript" src="https://www.thewindowsclub.com/wp-content/themes/noozbeat/js/jquery.matchHeight-min.js?ver=0.7.0" id="matchHeight-js"></script>
<script type="text/javascript" src="https://www.thewindowsclub.com/wp-content/themes/noozbeat/js/scripts.js?ver=1.0" id="noozbeat-front-scripts-js"></script>
<script type="text/javascript" id="q2w3_fixed_widget-js-extra">
/* <![CDATA[ */
var q2w3_sidebar_options = [{"sidebar":"blog","margin_top":10,"margin_bottom":0,"stop_id":"","screen_max_width":0,"screen_max_height":0,"width_inherit":false,"refresh_interval":1500,"window_load_hook":false,"disable_mo_api":false,"widgets":["text-422067541"]},{"sidebar":"page","margin_top":10,"margin_bottom":0,"stop_id":"","screen_max_width":0,"screen_max_height":0,"width_inherit":false,"refresh_interval":1500,"window_load_hook":false,"disable_mo_api":false,"widgets":["text-422067550"]}];
/* ]]> */
</script>
<script type="text/javascript" src="https://www.thewindowsclub.com/wp-content/plugins/q2w3-fixed-widget/js/q2w3-fixed-widget.min.js?ver=5.2.0" id="q2w3_fixed_widget-js"></script>
<script type="text/javascript" id="jquery-lazyloadxt-js-extra">
/* <![CDATA[ */
var a3_lazyload_params = {"apply_images":"1","apply_videos":"1"};
/* ]]> */
</script>
<script type="text/javascript" src="//www.thewindowsclub.com/wp-content/plugins/a3-lazy-load/assets/js/jquery.lazyloadxt.extra.min.js?ver=2.4.3" id="jquery-lazyloadxt-js"></script>
<script type="text/javascript" src="//www.thewindowsclub.com/wp-content/plugins/a3-lazy-load/assets/js/jquery.lazyloadxt.srcset.min.js?ver=2.4.3" id="jquery-lazyloadxt-srcset-js"></script>
<script type="text/javascript" id="jquery-lazyloadxt-extend-js-extra">
/* <![CDATA[ */
var a3_lazyload_extend_params = {"edgeY":"100","horizontal_container_classnames":""};
/* ]]> */
</script>
<script type="text/javascript" src="//www.thewindowsclub.com/wp-content/plugins/a3-lazy-load/assets/js/jquery.lazyloadxt.extend.js?ver=2.4.3" id="jquery-lazyloadxt-extend-js"></script>
<script type="text/javascript" src="https://www.thewindowsclub.com/wp-includes/js/wp-embed.min.js?ver=5.6.2" id="wp-embed-js"></script>
<script type="text/javascript" id="feedzy-rss-feeds-lazy-js-extra">
/* <![CDATA[ */
var feedzy = {"url":"https:\/\/www.thewindowsclub.com\/wp-json\/feedzy\/v1\/lazy\/","rest_nonce":"42fef0d6a0","nonce":"815222a0a9"};
var feedzy = {"url":"https:\/\/www.thewindowsclub.com\/wp-json\/feedzy\/v1\/lazy\/","rest_nonce":"42fef0d6a0","nonce":"815222a0a9"};
/* ]]> */
</script>
<script type="text/javascript" src="https://www.thewindowsclub.com/wp-content/plugins/feedzy-rss-feeds/js/feedzy-lazy.js?ver=3.5.2" id="feedzy-rss-feeds-lazy-js"></script>

		<div id="ss-all-networks-popup" class="ss-popup-overlay" data-nonce="454dddeeea">
			<div class="ss-popup">

				<div class="ss-popup-heading">
					<span>Share via</span>
					<a href="#" class="ss-close-modal" rel="nofollow noopener">
						<svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M17.883 16.667l7.058-7.058c0.517-0.517 0.517-1.367 0-1.883s-1.367-0.517-1.883 0l-7.058 7.058-7.058-7.058c-0.517-0.517-1.367-0.517-1.883 0s-0.517 1.367 0 1.883l7.058 7.058-7.058 7.058c-0.517 0.517-0.517 1.367 0 1.883 0.258 0.258 0.6 0.392 0.942 0.392s0.683-0.133 0.942-0.392l7.058-7.058 7.058 7.058c0.258 0.258 0.6 0.392 0.942 0.392s0.683-0.133 0.942-0.392c0.517-0.517 0.517-1.367 0-1.883l-7.058-7.058z"></path></svg>					</a>
				</div><!-- END .ss-popup-heading -->

				<div class="ss-popup-content">
					<div class="ss-popup-networks ss-clearfix">
						
							<div class="ss-popup-network ss-popup-facebook">
								<a href="#" data-ss-ss-link="https://www.facebook.com/sharer.php?t=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010&amp;u=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10" data-id="facebook" class="ss-facebook-color" data-ss-ss-network-id="facebook" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" data-has-api="true" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M32 16.098C32 7.208 24.837 0 16 0S0 7.207 0 16.098C0 24.133 5.851 30.792 13.5 32V20.751H9.437v-4.653H13.5V12.55c0-4.034 2.389-6.263 6.043-6.263 1.751 0 3.582.315 3.582.315v3.961h-2.018c-1.987 0-2.607 1.241-2.607 2.514v3.02h4.438l-.71 4.653H18.5V32C26.149 30.792 32 24.133 32 16.098z"></path></svg></span>
									<span>Facebook</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-twitter">
								<a href="#" data-ss-ss-link="https://twitter.com/intent/tweet?text=How+to+run+.sh+or+Shell+Script+file+in+Windows+10&amp;url=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10" data-id="twitter" class="ss-twitter-color" data-ss-ss-network-id="twitter" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M28.75 9.5c0 0.25 0 0.563 0 0.813 0 8.688-6.625 18.688-18.688 18.688-3.688 0-7.188-1.063-10.063-2.938 0.5 0.063 1.063 0.063 1.563 0.063 3.063 0 5.938-1 8.188-2.813-2.875 0-5.313-1.938-6.188-4.563 0.438 0.125 0.813 0.125 1.25 0.125 0.625 0 1.188-0.063 1.75-0.188-3-0.625-5.25-3.313-5.25-6.438 0-0.063 0-0.063 0-0.125 0.875 0.5 1.875 0.813 2.938 0.813-1.75-1.125-2.938-3.188-2.938-5.438 0-1.188 0.375-2.313 0.938-3.313 3.188 4 8.063 6.625 13.5 6.875-0.125-0.5-0.188-1-0.188-1.5 0-3.625 2.938-6.563 6.563-6.563 1.938 0 3.625 0.813 4.813 2.063 1.5-0.313 2.938-0.813 4.188-1.563-0.5 1.5-1.563 2.813-2.875 3.625 1.313-0.188 2.563-0.5 3.75-1.063-0.875 1.313-2 2.5-3.25 3.438z"></path></svg></span>
									<span>Twitter</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-linkedin">
								<a href="#" data-ss-ss-link="https://www.linkedin.com/shareArticle?title=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010&amp;url=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10&amp;mini=true" data-id="linkedin" class="ss-linkedin-color" data-ss-ss-network-id="linkedin" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M29.632 0C30.939 0 32 1.032 32 2.307v27.384C32 30.966 30.939 32 29.632 32H2.36C1.058 32 0 30.966 0 29.69V2.308C0 1.032 1.058 0 2.36 0h27.272zM9.149 11.638h-4.77V27h4.77V11.638zm12.133-.382c-2.318 0-3.874 1.273-4.509 2.48h-.066v-2.098H12.14V27h4.76v-7.599c0-2.004.378-3.946 2.858-3.946 2.447 0 2.475 2.29 2.475 4.072V27H27v-8.423c0-4.138-.893-7.32-5.718-7.32v-.001zM6.764 4A2.766 2.766 0 004 6.769a2.765 2.765 0 105.528 0A2.767 2.767 0 006.765 4h-.001z"></path></svg></span>
									<span>LinkedIn</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-mix">
								<a href="#" data-ss-ss-link="https://mix.com/add?url=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10" data-id="mix" class="ss-mix-color" data-ss-ss-network-id="mix" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="28" height="32" viewBox="0 0 28 32" xmlns="http://www.w3.org/2000/svg"><path d="M0 4v21.806c0 3.512 5.5 3.631 5.5 0v-14.912c0.494-3.306 5.5-3.15 5.5 0.406v10.956c0 3.619 6 3.625 6 0v-7.256c0.331-3.419 5.5-3.281 5.5 0.269v1.487c0 3.744 5.5 3.538 5.5 0v-12.756h-28z"></path></svg></span>
									<span>Mix</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-pinterest">
								<a href="#" data-ss-ss-link="https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10&amp;media=https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Shell-script-files-from-Command-Prompt.png&amp;description=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010" data-id="pinterest" class="ss-pinterest-color" data-ss-ss-network-id="pinterest" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" data-has-api="true" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M10.625 12.25c0-1.375 0.313-2.5 1.063-3.438 0.688-0.938 1.563-1.438 2.563-1.438 0.813 0 1.438 0.25 1.875 0.813s0.688 1.25 0.688 2.063c0 0.5-0.125 1.125-0.313 1.813-0.188 0.75-0.375 1.625-0.688 2.563-0.313 1-0.563 1.75-0.688 2.313-0.25 1-0.063 1.875 0.563 2.625 0.625 0.688 1.438 1.063 2.438 1.063 1.75 0 3.188-1 4.313-2.938 1.125-2 1.688-4.375 1.688-7.188 0-2.125-0.688-3.875-2.063-5.25-1.375-1.313-3.313-2-5.813-2-2.813 0-5.063 0.875-6.75 2.688-1.75 1.75-2.625 3.875-2.625 6.375 0 1.5 0.438 2.75 1.25 3.75 0.313 0.313 0.375 0.688 0.313 1.063-0.125 0.313-0.25 0.813-0.375 1.5-0.063 0.25-0.188 0.438-0.375 0.5s-0.375 0.063-0.563 0c-1.313-0.563-2.25-1.438-2.938-2.75s-1-2.813-1-4.5c0-1.125 0.188-2.188 0.563-3.313s0.875-2.188 1.625-3.188c0.75-1.063 1.688-1.938 2.688-2.75 1.063-0.813 2.313-1.438 3.875-1.938 1.5-0.438 3.125-0.688 4.813-0.688 1.813 0 3.438 0.313 4.938 0.938 1.5 0.563 2.813 1.375 3.813 2.375 1.063 1.063 1.813 2.188 2.438 3.5 0.563 1.313 0.875 2.688 0.875 4.063 0 3.75-0.938 6.875-2.875 9.313-1.938 2.5-4.375 3.688-7.375 3.688-1 0-1.938-0.188-2.813-0.688-0.875-0.438-1.5-1-1.875-1.688-0.688 2.938-1.125 4.688-1.313 5.25-0.375 1.438-1.25 3.188-2.688 5.25h-1.313c-0.25-2.563-0.188-4.688 0.188-6.375l2.438-10.313c-0.375-0.813-0.563-1.813-0.563-3.063z"></path></svg></span>
									<span>Pinterest</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-tumblr">
								<a href="#" data-ss-ss-link="https://www.tumblr.com/widgets/share/tool?canonicalUrl=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10&amp;title=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010&amp;posttype=link" data-id="tumblr" class="ss-tumblr-color" data-ss-ss-network-id="tumblr" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" data-has-api="true" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M6.125 13.125v-4.563c1.25-0.375 2.375-1 3.25-1.75s1.625-1.688 2.125-2.75c0.563-1.063 0.938-2.438 1.125-4.063h4.563v8.063h7.625v5.063h-7.625v8.188c0 1.875 0.125 3.063 0.313 3.563 0.188 0.563 0.563 0.938 1.063 1.25 0.75 0.438 1.563 0.688 2.438 0.688 1.625 0 3.25-0.563 4.875-1.625v5.063c-1.375 0.625-2.625 1.125-3.75 1.375-1.063 0.25-2.313 0.375-3.563 0.375-1.5 0-2.75-0.188-3.875-0.563s-2.125-0.875-2.875-1.563c-0.813-0.688-1.375-1.438-1.688-2.188s-0.438-1.875-0.438-3.375v-11.188z"></path></svg></span>
									<span>Tumblr</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-skype">
								<a href="#" data-ss-ss-link="https://web.skype.com/share?url=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10" data-id="skype" class="ss-skype-color" data-ss-ss-network-id="skype" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M30.875 19.375c0.25-1 0.313-2.125 0.313-3.188 0-8.313-6.688-15.063-15-15.063-0.875 0-1.75 0.063-2.563 0.188-1.375-0.813-2.938-1.313-4.688-1.313-4.813 0-8.688 3.938-8.688 8.75 0 1.563 0.438 3.125 1.188 4.375-0.188 1-0.313 2-0.313 3.063 0 8.313 6.75 15 15.063 15 0.938 0 1.813-0.063 2.75-0.25 1.188 0.688 2.625 1.063 4.125 1.063 4.813 0 8.688-3.938 8.688-8.75 0-1.375-0.313-2.688-0.875-3.875zM23.75 23.313c-0.688 1-1.688 1.75-3.063 2.313-1.313 0.563-2.875 0.813-4.688 0.813-2.125 0-3.938-0.375-5.375-1.125-1-0.5-1.875-1.25-2.5-2.188s-0.938-1.813-0.938-2.688c0-0.563 0.188-1.063 0.625-1.438s0.938-0.563 1.563-0.563c0.5 0 0.938 0.125 1.313 0.438s0.688 0.75 0.875 1.313c0.313 0.563 0.563 1.125 0.875 1.5s0.75 0.75 1.25 1c0.563 0.25 1.313 0.375 2.188 0.375 1.25 0 2.313-0.25 3.063-0.813 0.75-0.5 1.125-1.125 1.125-1.875 0-0.563-0.188-1.063-0.625-1.438-0.375-0.375-0.938-0.625-1.563-0.875-0.688-0.188-1.625-0.438-2.75-0.688-1.563-0.313-2.938-0.688-4-1.188-1.063-0.438-1.938-1.063-2.563-1.875s-1-1.813-1-3c0-1.125 0.375-2.188 1.063-3.063s1.625-1.563 2.938-2c1.25-0.5 2.688-0.688 4.375-0.688 1.375 0 2.563 0.125 3.5 0.438 1 0.313 1.875 0.75 2.5 1.25 0.688 0.5 1.188 1.063 1.5 1.625s0.438 1.188 0.438 1.75c0 0.5-0.188 1-0.625 1.438-0.375 0.438-0.938 0.625-1.563 0.625-0.5 0-0.938-0.125-1.25-0.375s-0.563-0.688-0.938-1.188c-0.375-0.75-0.813-1.313-1.313-1.688s-1.375-0.563-2.5-0.563c-1.125 0-2 0.188-2.625 0.625-0.625 0.375-0.938 0.875-0.938 1.438 0 0.313 0.063 0.625 0.313 0.875 0.188 0.25 0.5 0.5 0.875 0.688s0.813 0.375 1.188 0.438c0.438 0.125 1.125 0.313 2.125 0.563 1.188 0.25 2.313 0.5 3.313 0.813 1 0.375 1.875 0.75 2.563 1.188 0.75 0.5 1.313 1.063 1.688 1.813 0.438 0.688 0.625 1.625 0.625 2.625 0 1.25-0.375 2.375-1.063 3.375z"></path></svg></span>
									<span>Skype</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-buffer">
								<a href="#" data-ss-ss-link="https://buffer.com/add?url=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10&amp;text=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010" data-id="buffer" class="ss-buffer-color" data-ss-ss-network-id="buffer" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" data-has-api="true" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M31.438 24.313c-0.063-0.063-0.188-0.125-0.25-0.188-0.813-0.375-1.688-0.75-2.5-1.125-0.688-0.375-1.438-0.375-2.188 0-3.125 1.438-6.25 2.938-9.375 4.375-0.75 0.313-1.5 0.375-2.188 0-3.125-1.438-6.313-2.938-9.438-4.375-0.75-0.375-1.5-0.375-2.25 0s-1.563 0.75-2.313 1.063c-0.25 0.125-0.625 0.25-0.625 0.625 0 0.313 0.375 0.375 0.625 0.5 4.625 2.188 9.25 4.375 13.938 6.5 0.75 0.375 1.5 0.375 2.188 0.063 4.688-2.188 9.375-4.375 14.063-6.563 0.125-0.063 0.25-0.125 0.313-0.188 0.313-0.188 0.313-0.5 0-0.688zM0.5 7.688c0.125 0.063 0.313 0.188 0.438 0.25 4.688 2.125 9.313 4.313 13.938 6.5 0.75 0.313 1.5 0.313 2.25 0 4.625-2.188 9.313-4.375 13.938-6.5 0.125-0.125 0.313-0.188 0.438-0.313 0.25-0.125 0.25-0.375 0-0.563-0.125-0.125-0.313-0.188-0.438-0.313-4.625-2.125-9.25-4.313-13.875-6.438-0.813-0.375-1.563-0.375-2.375 0-4.625 2.125-9.25 4.313-13.875 6.5-0.188 0.063-0.313 0.125-0.438 0.188-0.25 0.188-0.25 0.5 0 0.688zM31.438 15.688c-0.063-0.063-0.188-0.125-0.25-0.188-0.813-0.375-1.688-0.75-2.5-1.125-0.688-0.375-1.438-0.375-2.188 0-3.125 1.438-6.25 2.938-9.375 4.375-0.75 0.313-1.5 0.313-2.188 0-3.125-1.438-6.313-2.938-9.438-4.375-0.75-0.375-1.5-0.375-2.25 0s-1.563 0.75-2.313 1.063c-0.25 0.125-0.625 0.25-0.625 0.563 0 0.375 0.375 0.438 0.625 0.563 4.625 2.188 9.25 4.375 13.938 6.5 0.75 0.375 1.5 0.375 2.188 0.063 4.688-2.188 9.375-4.375 14.063-6.563 0.125-0.063 0.25-0.125 0.313-0.188 0.313-0.188 0.313-0.5 0-0.688z"></path></svg></span>
									<span>Buffer</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-pocket">
								<a href="#" data-ss-ss-link="https://getpocket.com/save?url=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10" data-id="pocket" class="ss-pocket-color" data-ss-ss-network-id="pocket" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M32 5.5c0-0.875 0.063-1.688-0.438-2.438-0.375-0.563-1-1.063-1.625-1.25-0.875-0.25-1.813-0.188-2.625-0.125-3.75 0-7.563-0.063-11.313-0.063-0.438 0-0.813 0-1.25 0-0.5 0-1 0-1.563 0-1.813 0-3.688 0-5.563 0-0.938 0-1.875 0-2.813 0-0.5 0-1 0-1.5 0-0.438 0-0.813 0-1.188 0.125-1.313 0.375-2.125 1.625-2.125 3 0 1.875 0 3.75 0 5.625 0 1.813-0.063 3.688 0.063 5.563 0.125 1.688 0.625 3.438 1.313 5 1.313 2.813 3.438 5.188 6.063 6.875 2.875 1.813 6.313 2.688 9.688 2.438 3.313-0.25 6.5-1.563 9.063-3.688 2.438-1.938 4.188-4.563 5.125-7.5 0.5-1.688 0.688-3.5 0.688-5.25 0-1.813 0-3.688 0-5.563 0-0.938 0-1.875 0-2.75zM25.625 12.75c-0.188 0.813-1 1.375-1.563 1.938-1.438 1.375-2.875 2.75-4.313 4.063-0.75 0.75-1.438 1.438-2.188 2.125-0.563 0.5-1.313 0.75-2.063 0.563-0.875-0.188-1.5-1-2.063-1.563-0.75-0.688-1.438-1.375-2.125-2-1.438-1.375-2.875-2.75-4.313-4.188-1.063-1.063-0.875-3 0.625-3.625 0.688-0.25 1.5-0.188 2.063 0.188 0.375 0.313 0.75 0.625 1.063 1 0.375 0.313 0.75 0.688 1.063 1 1.438 1.375 2.75 2.75 4.188 4 1.625-1.5 3.25-3.063 4.875-4.625 0.688-0.625 1.313-1.5 2.313-1.688 0.75-0.125 1.563 0.188 2.063 0.75 0.438 0.563 0.625 1.375 0.375 2.063z"></path></svg></span>
									<span>Pocket</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-vkontakte">
								<a href="#" data-ss-ss-link="https://vk.com/share.php?url=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10" data-id="vkontakte" class="ss-vkontakte-color" data-ss-ss-network-id="vkontakte" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M30.938 22.063c-0.938-1.25-1.75-2-2.938-3.125-0.5-0.5-1.188-1-1.25-1.688-0.063-0.938 0.813-1.813 1.25-2.438 0.063-0.063 0.125-0.125 0.188-0.188s0.063-0.063 0.125-0.125c0-0.063 0.063-0.063 0.063-0.125 0.063-0.063 0.063-0.125 0.125-0.125 0-0.063 0.063-0.063 0.063-0.063 0.063-0.063 0.063-0.125 0.125-0.188 0.813-1.063 1.625-2 2.438-3.25 0.25-0.438 1.063-2 0.813-2.625-0.375-0.75-2.313-0.5-3.375-0.5-1.313 0-2.75-0.25-3.688 0.125-0.563 0.188-0.938 1.438-1.25 2.125-0.5 1.063-0.938 1.938-1.438 2.75 0 0.063-0.063 0.125-0.125 0.188 0 0 0 0 0 0 0 0.063-0.063 0.125-0.125 0.188 0 0 0 0 0 0-0.063 0.125-0.125 0.25-0.188 0.313 0 0.063-0.063 0.063-0.063 0.063 0 0.063-0.063 0.063-0.063 0.125-0.063 0.063-0.063 0.063-0.063 0.125-0.063 0-0.063 0.063-0.125 0.125 0 0-0.063 0.063-0.063 0.125-0.063 0-0.063 0.063-0.063 0.063-0.063 0.063-0.125 0.125-0.188 0.25-0.438 0.625-0.875 1.375-1.688 1.5-0.063-0.063-0.063-0.063-0.125-0.063 0 0 0-0.063 0-0.063-0.063 0-0.063 0-0.063 0 0-0.063-0.063-0.063-0.063-0.063s0 0-0.063-0.063c0 0 0 0 0 0s0-0.063-0.063-0.063c0 0 0 0 0 0 0-0.063-0.063-0.063-0.063-0.063s0-0.063 0-0.063c0 0-0.063 0-0.063-0.063 0 0 0 0 0 0 0-0.063 0-0.063-0.063-0.063 0 0 0-0.063 0-0.063s0 0 0-0.063c0 0-0.063 0-0.063 0 0-0.063 0-0.063 0-0.125 0 0 0 0 0 0-0.063-0.063-0.063-0.063-0.063-0.063 0-0.063 0-0.063 0-0.063s0-0.063 0-0.063c0 0 0-0.063-0.063-0.063 0 0 0-0.063 0-0.063s0 0 0-0.063c0 0 0 0 0-0.063 0 0 0 0 0 0 0-0.063 0-0.063-0.063-0.063 0-0.063 0-0.063 0-0.063 0-0.063 0-0.063 0-0.063 0-0.063 0-0.063 0-0.063 0-0.063 0-0.063 0-0.063 0-0.063 0-0.063 0-0.063 0-0.063 0-0.063 0-0.125 0 0 0 0 0 0 0-0.063 0-0.063 0-0.125 0 0 0 0 0 0 0-0.063 0-0.063 0-0.125 0 0-0.063 0-0.063-0.063 0 0 0-0.063 0-0.063s0-0.063 0-0.063c0 0 0-0.063 0-0.063s0-0.063 0-0.063c0 0 0-0.063 0-0.063 0-0.063 0.063-0.063 0.063-0.063 0-0.063 0-0.063 0-0.063 0-0.063 0-0.063 0-0.063 0-0.063 0-0.063 0-0.125 0 0 0 0 0 0 0-0.063 0-0.063 0-0.125 0 0 0 0 0 0 0-0.188 0-0.313 0-0.5 0 0 0-0.063 0-0.063 0-0.125 0-0.313 0.063-0.438 0-1.375 0.438-3.188-0.188-4.25-0.563-0.938-2.688-0.813-4.188-0.813-1.813 0-3.25 0.125-3.813 1.188 0.625 0.438 1.313 0.438 1.625 1.063 0.375 0.688 0.438 2.125 0.375 3.438 0 0.063 0 0.125 0 0.188 0 1.125-0.063 2.938-0.813 3.063s-1.375-1-1.813-1.563c-0.063-0.125-0.125-0.188-0.188-0.313 0 0-0.063-0.063-0.063-0.063-0.063-0.063-0.063-0.125-0.125-0.25 0 0-0.063-0.063-0.063-0.063-0.063-0.063-0.125-0.125-0.125-0.188-0.063-0.063-0.063-0.063-0.063-0.125-0.063-0.063-0.125-0.188-0.188-0.25-0.563-0.938-1.125-1.875-1.625-3.063-0.375-0.688-0.813-1.875-1.188-2.063-0.75-0.375-2.25-0.188-3.25-0.188-1.125 0-2.313-0.188-3 0.375 0 1.25 0.625 2.313 1.125 3.313 0.688 1.375 1.375 2.688 2.125 3.938 0 0.063 0.063 0.125 0.063 0.188 0.125 0.125 0.188 0.313 0.313 0.438 0 0.063 0.063 0.125 0.063 0.188 0.125 0.125 0.188 0.313 0.313 0.438 0 0.063 0.063 0.125 0.125 0.188 0.125 0.188 0.25 0.375 0.375 0.563 0 0 0 0 0 0 0.125 0.188 0.25 0.438 0.375 0.625 0.063 0.063 0.063 0.125 0.125 0.125 0.125 0.188 0.188 0.313 0.313 0.438 0 0.063 0.063 0.125 0.125 0.188 0.063 0.125 0.188 0.313 0.313 0.438 0 0.063 0.063 0.125 0.125 0.188 0.125 0.188 0.25 0.375 0.438 0.563 1.938 2.438 4.125 4.75 8.438 5.25 1.375 0.125 3.375 0.25 3.813-0.563 0.625-1-0.063-3.375 1.313-3.563 0.938-0.188 1.75 1.25 2.313 1.813 0.938 1.063 2.063 2.188 3.688 2.5 0 0 0.063 0 0.125 0 1.438-0.625 5.75 0.688 6-1.125 0.063-0.625-0.688-1.625-1.063-2.063z"></path></svg></span>
									<span>VKontakte</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-parler">
								<a href="#" data-ss-ss-link="https://parler.com/new-post?url=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10&amp;message=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010" data-id="parler" class="ss-parler-color" data-ss-ss-network-id="parler" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M18.669 26.66h-8v-2.718a2.603 2.603 0 012.605-2.604h5.398c4.416 0 8.006-3.581 8.006-7.981s-3.593-7.981-8.01-7.981h-.082l-1.696-.051H0A5.324 5.324 0 015.322 0h11.65l1.742.054C26.044.077 32 6.035 32 13.357c0 7.334-5.98 13.302-13.331 13.302z"></path><path d="M5.322 32A5.321 5.321 0 010 26.678V15.837a5.171 5.171 0 015.171-5.171h13.501a2.662 2.662 0 010 5.324H7.952a2.627 2.627 0 00-2.627 2.628V32h-.003z"></path></svg></span>
									<span>Parler</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-xing">
								<a href="#" data-ss-ss-link="https://www.xing.com/app/user?url=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10&amp;op=share" data-id="xing" class="ss-xing-color" data-ss-ss-network-id="xing" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M7.688 22.438h-4.625c-0.25 0-0.438-0.125-0.563-0.313s-0.125-0.5 0-0.75l4.875-8.625c0 0 0 0 0-0.063l-3.125-5.375c-0.125-0.25-0.125-0.5 0-0.688s0.313-0.313 0.625-0.313h4.625c0.688 0 1.063 0.438 1.25 0.875 0 0 3.188 5.5 3.188 5.5-0.188 0.375-5 8.813-5 8.813-0.25 0.438-0.563 0.938-1.25 0.938zM29.5 1l-10.188 18.063c0 0 0 0.063 0 0.063l6.5 11.875c0.125 0.25 0.125 0.5 0 0.688s-0.313 0.313-0.625 0.313h-4.625c-0.688 0-1-0.5-1.25-0.875 0 0-6.563-12-6.563-12.063 0.313-0.563 10.25-18.188 10.25-18.188 0.25-0.438 0.563-0.875 1.25-0.875h4.688c0.25 0 0.5 0.125 0.563 0.313 0.125 0.188 0.125 0.438 0 0.688z"></path></svg></span>
									<span>Xing</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-reddit">
								<a href="#" data-ss-ss-link="https://www.reddit.com/submit?title=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010&amp;url=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10" data-id="reddit" class="ss-reddit-color" data-ss-ss-network-id="reddit" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M32 15.75c0-1.75-1.375-3.125-3.125-3.125-1 0-1.875 0.438-2.438 1.188-2.5-1.813-6-2.938-9.938-3l2.313-6.875 5.75 1.375c0.125 0 0.188 0 0.25 0 0.063 1.313 1.125 2.375 2.5 2.375s2.438-1.125 2.438-2.5c0-1.375-1.063-2.438-2.438-2.438-1.063 0-1.875 0.563-2.313 1.438 0 0-0.063-0.063-0.125-0.063l-6.313-1.5c-0.313-0.063-0.625 0.125-0.688 0.375l-2.688 7.813c-3.813 0.125-7.188 1.188-9.688 2.938-0.563-0.688-1.375-1.125-2.375-1.125-1.75 0-3.125 1.375-3.125 3.125 0 1.25 0.75 2.375 1.875 2.875-0.125 0.438-0.188 0.938-0.188 1.438 0 5.125 6.375 9.313 14.25 9.313s14.25-4.188 14.25-9.313c0-0.438-0.063-0.938-0.188-1.375 1.188-0.5 2-1.625 2-2.938zM8.688 18.25c0-1.25 1.063-2.313 2.313-2.313s2.313 1.063 2.313 2.313c0 1.25-1.063 2.313-2.313 2.313s-2.313-1.063-2.313-2.313zM21.188 24.625c-1.063 1.063-2.75 1.563-5.188 1.563s-4.125-0.5-5.188-1.563c-0.125-0.125-0.125-0.375 0-0.563 0.125-0.125 0.375-0.125 0.5 0 0.938 0.938 2.438 1.375 4.688 1.375 2.188 0 3.75-0.438 4.688-1.375 0.125-0.125 0.375-0.125 0.5 0 0.125 0.188 0.125 0.438 0 0.563zM21.063 20.563c-1.313 0-2.375-1-2.375-2.313 0-1.25 1.063-2.313 2.375-2.313 1.25 0 2.25 1.063 2.25 2.313 0 1.313-1 2.313-2.25 2.313z"></path></svg></span>
									<span>Reddit</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-flipboard">
								<a href="#" data-ss-ss-link="https://share.flipboard.com/bookmarklet/popout?v=2&amp;title=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010&amp;url=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10" data-id="flipboard" class="ss-flipboard-color" data-ss-ss-network-id="flipboard" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M4.313 2.313v23.375h7.813v-7.813h7.75v-7.75h7.813v-7.813z"></path></svg></span>
									<span>Flipboard</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-myspace">
								<a href="#" data-ss-ss-link="https://myspace.com/post?u=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10" data-id="myspace" class="ss-myspace-color" data-ss-ss-network-id="myspace" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M26.438 17.438c3.063 0 5.563 2.438 5.563 5.563 0 1 0 2.813 0 2.813h-11.188c0 0 0-1.813 0-2.813 0-3.125 2.5-5.563 5.625-5.563zM21.313 11.313c0-2.813 2.25-5.125 5.125-5.125 2.813 0 5.125 2.313 5.125 5.125 0 2.875-2.313 5.125-5.125 5.125-2.875 0-5.125-2.25-5.125-5.125zM14.875 18.313c2.75 0 5 2.25 5 5 0 0.875 0 2.5 0 2.5h-9.938c0 0 0-1.625 0-2.5 0-2.75 2.188-5 4.938-5zM10.313 12.75c0-2.563 2.063-4.625 4.563-4.625 2.563 0 4.625 2.063 4.625 4.625 0 2.5-2.063 4.563-4.625 4.563s-4.563-2.063-4.563-4.563zM4.438 19.063c2.5 0 4.5 2 4.5 4.5 0 0.813 0 2.25 0 2.25h-8.938c0 0 0-1.438 0-2.25 0-2.5 2-4.5 4.438-4.5zM0.313 14.063c0-2.313 1.875-4.125 4.125-4.125 2.313 0 4.125 1.813 4.125 4.125 0 2.25-1.813 4.125-4.125 4.125-2.25 0-4.125-1.875-4.125-4.125z"></path></svg></span>
									<span>MySpace</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-delicious">
								<a href="#" data-ss-ss-link="https://del.icio.us/post?url=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10&amp;title=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010" data-id="delicious" class="ss-delicious-color" data-ss-ss-network-id="delicious" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M32 16h-16v16h-16v-16h16v-16h16z"></path></svg></span>
									<span>Delicious</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-amazon">
								<a href="#" data-ss-ss-link="https://www.amazon.com/gp/wishlist/static-add?u=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10&amp;t=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010" data-id="amazon" class="ss-amazon-color" data-ss-ss-network-id="amazon" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M27.696 26.643c0.536-0.268 0.946 0.143 0.393 0.857s-5 4.786-12.464 4.786-13.179-5.107-14.929-7.214c-0.482-0.554 0.071-0.804 0.393-0.589 5.232 3.179 13.411 8.411 26.607 2.161zM31.393 24.589c0.268 0.357 0 1.929-0.464 3.071-0.464 1.125-1.143 1.911-1.518 2.214-0.393 0.321-0.679 0.196-0.464-0.268s1.375-3.321 0.911-3.929c-0.464-0.589-2.643-0.304-3.429-0.232-0.768 0.071-0.929 0.143-1-0.018-0.161-0.411 1.554-1.107 2.679-1.25 1.125-0.125 2.929-0.054 3.286 0.411zM24.357 16.679c0 1.964 2.304 3.768 2.304 3.768l-4.054 4c-1.589-1.5-2.786-2.75-2.786-2.75-0.179-0.179-0.321-0.393-0.446-0.589-3.232 5.054-13.107 4.732-13.107-3.089 0-7.286 8.625-8.268 12.107-8.393v-2.268c0-0.482 0.179-2.679-2.536-2.679 0 0-2.714 0-3.875 3.536l-5.25-0.482c0-3.518 3.339-7.446 9.625-7.446 6.268 0 8.018 4.071 8.018 5.875v10.518zM12.357 17.054c0 3.625 6.018 4.482 6.018-1.232v-2.893c-2.411 0.071-6.018 0.75-6.018 4.125z"></path></svg></span>
									<span>Amazon</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-digg">
								<a href="#" data-ss-ss-link="https://digg.com/submit?title=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010&amp;url=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10" data-id="digg" class="ss-digg-color" data-ss-ss-network-id="digg" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M9.625 10.875h3.188v10.875h-3.188zM5.125 6.375h3.188v15.375h-8.313v-10.875h5.125zM5.125 13.438h-1.938v5.75h1.938zM9.625 9.625h3.188v-3.25h-3.188zM14.063 10.875h8.313v14.75h-8.313v-2.563h5.125v-1.313h-5.125zM17.25 19.188h1.938v-5.75h-1.938zM32 10.875v14.75h-8.313v-2.563h5.125v-1.313h-5.125v-10.875zM28.813 13.438h-1.938v5.75h1.938z"></path></svg></span>
									<span>Digg</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-evernote">
								<a href="#" data-ss-ss-link="https://www.evernote.com/clip.action?url=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10" data-id="evernote" class="ss-evernote-color" data-ss-ss-network-id="evernote" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M9.546 8.030c0.234 0 0.476-0.188 0.476-0.418 0-0.002 0-4.862 0-4.862 0-0.79 0.466-1.876 0.45-1.86l-7.94 7.774c0 0 0.928-0.634 2.468-0.634h4.546zM25 3h-5c-0.13-0.886-0.876-2.18-1.572-2.46-1.852-0.746-3.68-0.566-4.414-0.36-0.584 0.164-1.23 0.498-1.59 1.014-0.242 0.344-0.422 0.784-0.424 1.402 0 0 0 2.78 0 5.904 0 1.062-0.438 1.5-1.438 1.5h-6.562c-0.64 0-2 0.124-2 2.456 0 0.838 1.15 5.698 2.006 7.462 0 0 0.494 1.52 2.464 2.082 0 0 3.378 0.874 4.532 1 1.052 0.114 2.998 0 2.998-3v-2c0-0.552 0.448-1 1-1s1 0.448 1 1v1c0 3 3 2.968 3 2.968h2.124c1.876 0 2.76 1.032 2.76 3.032 0 3.432-1.108 3.928-2.93 4h-1.916c-0.538 0-1.038-0.436-1.038-0.976v-1.024c0-1.024 1-1 1-1s0.968 0 1 0c0.552 0 1-0.448 1-1s-0.448-1-1-1h-1.938c-1.14 0-2.062 0.922-2.062 2.060v1.94c0 3 2.334 4 4 4 0 0 1.572 0 2.458 0 3.5 0 7.542 0 7.542-12.722v-11.278c0-3-2.358-5-5-5zM26 16h-6v-1c0-1.656 1.344-3 3-3s3 1.344 3 3v1z"></path></svg></span>
									<span>Evernote</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-blogger">
								<a href="#" data-ss-ss-link="https://www.blogger.com/blog-this.g?u=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10&amp;n=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010" data-id="blogger" class="ss-blogger-color" data-ss-ss-network-id="blogger" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M29.75 12.188h-1.375c-1.375 0-2.125-0.938-2.125-1.938v-0.875c0-4.563-5.063-9.375-9.375-9.375h-6.75c-5.688 0-10.125 4.5-10.125 10.188v12.125c0 5.313 4.563 9.688 9.313 9.688h12.813c5.25 0 9.875-4.438 9.875-9.813v-7.688c0-1.438-0.5-2.313-2.25-2.313zM10.125 8.313h5.813c1 0 1.875 0.875 1.875 1.938 0 1-0.875 1.938-1.875 1.938h-5.813c-1 0-1.875-0.938-1.875-1.938s0.875-1.938 1.875-1.938zM21.688 23.688h-11.563c-1 0-1.875-0.75-1.875-1.75 0-1.063 0.875-1.75 1.875-1.75h11.563c1 0 1.875 0.688 1.875 1.75 0 1-0.875 1.75-1.875 1.75z"></path></svg></span>
									<span>Blogger</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-livejournal">
								<a href="#" data-ss-ss-link="http://www.livejournal.com/update.bml?event=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10&amp;subject=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010" data-id="livejournal" class="ss-livejournal-color" data-ss-ss-network-id="livejournal" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M11 3.125c0 0 0 0 0 0s0 0 0 0 0 0 0 0zM16.938 1.875c-2.125 0-4.125 0.438-5.938 1.25 0.125 0.063 0.188 0.125 0.313 0.25 0.313 0.313 0.625 0.625 0.938 0.938 0.063 0.063 0.063 0.063 0.063 0.063l10.75 10.75c-3.313 1.938-5.875 4.563-7.75 8l-10.813-10.813c-0.063-0.063-0.063-0.063-0.125-0.125-0.313-0.375-0.688-0.688-1-1-0.063-0.063-0.125-0.125-0.188-0.25 1.625-3.563 4.188-6.188 7.875-7.75-0.063-0.063-0.063-0.063-0.063-0.063s0 0 0 0c-0.938-0.938-1.875-1.813-2.75-2.75-0.375-0.313-0.688-0.438-1.125-0.188-0.563 0.25-1.063 0.563-1.563 0.875-1.75 1.188-3.188 2.625-4.375 4.313-0.375 0.563-0.75 1.125-1.063 1.813-0.188 0.375-0.188 0.625 0.188 0.938 0.938 0.938 1.875 1.875 2.813 2.813-0.813 1.813-1.188 3.875-1.188 5.938 0 8.313 6.75 15.063 15 15.063 8.313 0 15.063-6.75 15.063-15.063 0-8.25-6.75-15-15.063-15zM18.5 24.313c1.25-2.875 3.25-4.813 6-6.125 0.5 2.563 1 5 1.5 7.688-2.625-0.563-5-1.063-7.5-1.563z"></path></svg></span>
									<span>LiveJournal</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-baidu">
								<a href="#" data-ss-ss-link="http://cang.baidu.com/do/add?iu=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10&amp;it=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010" data-id="baidu" class="ss-baidu-color" data-ss-ss-network-id="baidu" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M20.5 10.188c2.563 0.375 4.188-2.375 4.563-4.438 0.313-2.063-1.375-4.5-3.188-4.938-1.813-0.375-4.063 2.5-4.25 4.438-0.25 2.313 0.313 4.625 2.875 4.938zM5.75 16.875c3.5-0.75 3-4.938 2.938-5.813-0.188-1.438-1.875-3.875-4.063-3.688-2.813 0.25-3.25 4.313-3.25 4.313-0.375 1.875 0.938 5.938 4.375 5.188zM12.188 9.875c1.938 0 3.5-2.188 3.5-4.938s-1.563-4.938-3.5-4.938c-1.875 0-3.438 2.188-3.438 4.938s1.563 4.938 3.438 4.938zM9.438 24.125c-0.063 0.25-0.313 1-0.125 1.688 0.375 1.438 1.688 1.5 1.688 1.5h1.813v-4.438h-1.938c-0.875 0.25-1.313 0.938-1.438 1.25zM30.688 13.688c0-1-0.813-4-3.875-4-3.125 0-3.5 2.875-3.5 4.875 0 1.875 0.188 4.563 4 4.438 3.75-0.063 3.375-4.313 3.375-5.313zM26.813 22.438c0 0-4-3.063-6.313-6.375-3.125-4.938-7.625-2.938-9.125-0.438s-3.813 4.063-4.125 4.5c-0.313 0.375-4.813 2.813-3.813 7.188 1 4.438 4.5 4.313 4.5 4.313s2.563 0.25 5.5-0.375c3-0.688 5.563 0.125 5.563 0.125s7 2.375 8.875-2.125c1.875-4.5-1.063-6.813-1.063-6.813zM14.875 29.125h-4.5c-1.938-0.438-2.75-1.75-2.813-2-0.125-0.188-0.688-1.25-0.375-3.063 0.813-2.75 3.25-2.938 3.25-2.938h2.375v-3l2.063 0.063zM23.313 29.063h-5.188c-2.063-0.5-2.125-1.938-2.125-1.938v-5.75l2.125-0.063v5.188c0.125 0.563 0.813 0.688 0.813 0.688h2.125v-5.813h2.25z"></path></svg></span>
									<span>Baidu</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-mewe">
								<a href="#" data-ss-ss-link="https://mewe.com/share?link=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010%20https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10" data-id="mewe" class="ss-mewe-color" data-ss-ss-network-id="mewe" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="46" height="32" viewBox="0 0 46 32" xmlns="http://www.w3.org/2000/svg"><path d="M10.618 6.228a2.147 2.147 0 11-4.294 0 2.147 2.147 0 014.294 0zm10.455.007a2.148 2.148 0 11-4.292-.174 2.148 2.148 0 014.292.174zm12.356 0a2.15 2.15 0 11-4.301 0 2.15 2.15 0 014.301 0zm12.348 0a2.15 2.15 0 11-4.3 0 2.15 2.15 0 014.3 0zM0 12.117c0-.829.658-1.512 1.512-1.512h.317c.659 0 1.099.341 1.39.804l5.167 8.094 5.194-8.118c.317-.512.757-.78 1.363-.78h.316c.854 0 1.513.681 1.513 1.512v14.284a1.485 1.485 0 01-1.512 1.488 1.51 1.51 0 01-1.488-1.488V16.163L9.606 22.43c-.317.486-.708.78-1.268.78-.535 0-.926-.294-1.243-.78l-4.144-6.215v10.214c0 .829-.659 1.461-1.488 1.461a1.434 1.434 0 01-1.461-1.461v-14.31H0zm19 .498a1.585 1.585 0 01-.122-.586c0-.83.707-1.461 1.535-1.461.73 0 1.294.463 1.488 1.098l3.926 11.726 3.85-11.676c.245-.708.754-1.194 1.513-1.194h.218c.754 0 1.294.49 1.512 1.194l3.851 11.676 3.926-11.752c.222-.61.73-1.072 1.462-1.072.804 0 1.487.636 1.487 1.438-.01.21-.06.417-.146.61l-5.048 14.141c-.267.757-.829 1.243-1.561 1.243h-.29c-.731 0-1.27-.463-1.536-1.243L31.26 15.616l-3.803 11.141c-.267.78-.827 1.243-1.562 1.243h-.29c-.73 0-1.268-.463-1.562-1.243L19 12.615z"></path></svg></span>
									<span>MeWe</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-newsvine">
								<a href="#" data-ss-ss-link="https://www.newsvine.com/_tools/seed&amp;save?u=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10&amp;h=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010" data-id="newsvine" class="ss-newsvine-color" data-ss-ss-network-id="newsvine" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M17.125 27.375l2.75-2c0-0.125 0-0.188 0-0.25 0-1.25 1-2.313 2.25-2.313s2.313 1.063 2.313 2.313c0 1.25-1.063 2.25-2.313 2.25-0.438 0-0.875-0.125-1.188-0.375l-3.813 2.75v2.25h-2.25v-6.75l-3.875-2.813c-0.375 0.188-0.75 0.313-1.125 0.313-1.25 0-2.313-1.063-2.313-2.313s1.063-2.25 2.313-2.25c1.25 0 2.25 1 2.25 2.25 0 0.125 0 0.25-0.063 0.375l2.813 2.063v-6.75l-3.875-2.813c-0.375 0.188-0.75 0.313-1.125 0.313-1.25 0-2.313-1.063-2.313-2.313s1.063-2.25 2.313-2.25c1.25 0 2.25 1 2.25 2.25 0 0.125 0 0.313-0.063 0.438l2.813 2v-6.313l-3.938-2.875c-0.313 0.188-0.688 0.313-1.063 0.313-1.25 0-2.313-1-2.313-2.25s1.063-2.313 2.313-2.313c1.25 0 2.25 1.063 2.25 2.313 0 0.125 0 0.25-0.063 0.375l2.813 2.063v-5.063h2.25v9.563l2.75-2c0-0.125 0-0.25 0-0.313 0-1.25 1-2.313 2.25-2.313s2.313 1.063 2.313 2.313c0 1.25-1.063 2.25-2.313 2.25-0.438 0-0.813-0.125-1.188-0.313l-3.813 2.75v6.313l2.75-2c0-0.125 0-0.188 0-0.25 0-1.313 1-2.313 2.25-2.313s2.313 1 2.313 2.313c0 1.25-1.063 2.25-2.313 2.25-0.438 0-0.813-0.125-1.188-0.375l-3.813 2.813v6.688z"></path></svg></span>
									<span>NewsVine</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-yummly">
								<a href="#" data-ss-ss-link="https://www.yummly.com/urb/verify?url=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10&amp;title=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010&amp;yumtype=button" data-id="yummly" class="ss-yummly-color" data-ss-ss-network-id="yummly" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="49" height="32" viewBox="0 0 49 32" xmlns="http://www.w3.org/2000/svg"><path d="M4.576 0.128c-0.032 0.032-0.16 0.064-0.32 0.064-0.576 0.096-1.216 0.288-1.376 0.384-0.064 0.064-0.128 0.064-0.16 0.032s-0.032 0-0.032 0.064c0 0.064-0.032 0.064-0.064 0.064-0.096-0.096-1.504 0.672-1.888 1.024-0.16 0.16-0.32 0.288-0.32 0.256s-0.096 0.096-0.192 0.288c-0.16 0.256-0.192 0.416-0.192 0.672 0.032 0.224 0.096 0.448 0.16 0.512 0.032 0.064 0.064 0.096 0.032 0.096-0.096 0 0.064 0.288 0.384 0.768 0.16 0.224 0.32 0.416 0.384 0.416 0.032 0 0.096 0.032 0.064 0.064-0.032 0.128 0.384 0.416 0.576 0.416 0.128 0 0.32-0.128 0.544-0.32 0.16-0.192 0.352-0.32 0.352-0.32 0.032 0 0.192-0.096 0.384-0.224 0.704-0.48 1.6-0.608 1.856-0.288 0.064 0.064 0.16 0.128 0.192 0.096 0.064-0.032 0.064-0.032 0.032 0.032s-0.032 0.192 0 0.288c0.032 0.096 0.032 0.352 0 0.576-0.032 0.192-0.096 0.48-0.096 0.576-0.032 0.128-0.096 0.384-0.16 0.544-0.032 0.192-0.096 0.384-0.096 0.448-0.032 0.032-0.096 0.288-0.16 0.544-0.096 0.256-0.16 0.576-0.192 0.704s-0.064 0.256-0.064 0.288c-0.064 0.064-0.128 0.352-0.16 0.672-0.032 0.064-0.064 0.16-0.064 0.256-0.064 0.16-0.256 0.832-0.288 0.992 0 0.064-0.032 0.192-0.064 0.256-0.064 0.128-0.224 0.8-0.256 0.992-0.032 0.064-0.16 0.576-0.288 1.088-0.16 0.512-0.288 1.024-0.288 1.088-0.032 0.096-0.096 0.288-0.128 0.448-0.064 0.192-0.064 0.352-0.064 0.384 0.032 0.032 0.032 0.096-0.032 0.096-0.096 0.032-0.224 0.96-0.192 1.632 0 0.544 0.32 1.696 0.448 1.696 0.032 0 0.096 0.064 0.128 0.16 0.064 0.224 0.64 0.768 1.024 0.992 0.96 0.544 2.752 0.608 4.512 0.224 0.736-0.16 1.888-0.544 1.92-0.64 0-0.032 0.064-0.064 0.096-0.032 0.064 0.064 1.088-0.448 1.312-0.64 0.064-0.032 0.128-0.064 0.16-0.032 0.032 0-0.032 0.416-0.128 0.864-0.096 0.48-0.16 0.896-0.16 0.928 0 0.064-0.032 0.224-0.16 0.672 0 0.096-0.096 0.16-0.16 0.16-0.576 0-2.688 0.512-2.688 0.608 0 0.064-0.032 0.064-0.096 0.032s-1.184 0.384-1.28 0.512c-0.032 0.032-0.064 0.064-0.064 0s-0.672 0.288-0.768 0.384c0 0.032-0.064 0.096-0.096 0.096-0.16 0-0.704 0.352-0.672 0.416s0.032 0.064-0.032 0.032c-0.16-0.096-1.856 1.664-1.696 1.824 0.032 0.032 0 0.032-0.064 0.032-0.128 0-0.832 1.472-0.96 2.112-0.032 0.096-0.128 0.992-0.16 1.216-0.032 0.544 0.128 1.344 0.384 1.92 0.864 1.824 3.040 2.688 5.44 2.176 0.512-0.128 1.568-0.512 1.696-0.64 0.064-0.064 0.16-0.128 0.16-0.096 0.064 0.032 0.192 0 0.32-0.128 0.096-0.096 0.256-0.224 0.352-0.288 0.192-0.128 0.736-0.64 1.088-1.024 0.32-0.352 0.768-1.024 0.736-1.088-0.032-0.032-0.032-0.064 0.032-0.064s0.352-0.512 0.352-0.608c0-0.032 0.032-0.096 0.064-0.128 0.192-0.128 0.832-1.888 1.088-3.008 0.16-0.64 0.32-1.184 0.352-1.248 0.064-0.16 0.384-0.16 1.984 0.032 0.992 0.128 1.152 0.128 1.344 0.16 0.128 0.032 0.544 0.096 0.96 0.192 1.12 0.16 0.992 0.16 2.88 0.544 0.736 0.128 1.376 0.256 1.472 0.288 0.064 0 0.192 0.032 0.288 0.064 0.064 0.032 0.224 0.064 0.352 0.064 0.192 0.032 0.832 0.16 0.896 0.192 0.032 0 0.16 0.032 0.256 0.064 0.224 0.064 2.432 0.512 2.752 0.608 0.128 0 0.512 0.096 0.864 0.16 0.8 0.16 1.12 0.224 1.376 0.256 0.096 0 0.192 0.032 0.192 0.032 0 0.032 0.064 0.064 0.096 0.064 0.128 0 0.768 0.096 1.024 0.16 0.704 0.128 2.144 0.352 2.528 0.416 0.288 0.032 0.512 0.064 0.544 0.096 0.032 0 0.32 0.032 0.672 0.064 0.32 0.032 0.672 0.064 0.768 0.096 0.704 0.128 5.152 0.224 5.984 0.096 0.224-0.032 0.608-0.064 0.896-0.096s0.544-0.128 0.576-0.16c0.032-0.032 0.064-0.032 0.096-0.032 0.256 0.16 3.616-0.992 3.616-1.216 0-0.032 0.032-0.064 0.064-0.064 0.096 0.032 0.576-0.224 1.024-0.544 0.512-0.384 0.768-0.896 0.768-1.504 0-0.544-0.288-1.248-0.672-1.76-0.288-0.416-0.608-0.736-0.608-0.64 0 0.032-0.032 0-0.096-0.032-0.064-0.064-0.352 0.032-1.056 0.384-0.544 0.256-1.12 0.512-1.28 0.576s-0.416 0.16-0.544 0.224c-0.32 0.16-2.336 0.672-2.816 0.736-0.192 0.032-0.448 0.064-0.544 0.096-0.128 0-0.448 0.032-0.768 0.064-0.288 0.064-0.672 0.096-0.832 0.096-0.448 0.064-3.904 0.064-4.512 0-0.288 0-0.768-0.064-1.056-0.096-0.416-0.032-0.768-0.064-1.664-0.16-0.128 0-0.384-0.032-0.576-0.064-1.152-0.16-1.792-0.256-1.952-0.256-0.128-0.032-0.224-0.032-0.224-0.032 0-0.032-0.16-0.064-0.704-0.128-0.224-0.032-0.48-0.064-0.576-0.096-0.128-0.032-0.448-0.096-0.768-0.128-0.288-0.064-0.64-0.128-0.736-0.128-0.128-0.032-0.32-0.064-0.416-0.064-0.256-0.064-2.048-0.384-2.368-0.448-0.192-0.032-0.736-0.128-1.024-0.16-0.096 0-0.16-0.032-0.16-0.032 0-0.032-0.224-0.064-0.672-0.128-0.192 0-0.416-0.064-0.512-0.064-0.096-0.032-0.32-0.064-0.544-0.096-0.192-0.032-0.448-0.096-0.544-0.096-0.096-0.032-0.32-0.064-0.512-0.064-0.16-0.032-0.384-0.064-0.48-0.064-0.096-0.032-0.416-0.096-0.672-0.128-0.288-0.032-0.576-0.064-0.672-0.064-0.096-0.032-0.384-0.064-0.64-0.096-0.224-0.032-0.544-0.064-0.704-0.064-0.48-0.064-1.568-0.16-1.76-0.16-0.16 0.032-0.16 0-0.064-0.512 0.064-0.288 0.128-0.672 0.16-0.896 0.128-0.768 0.256-1.6 0.32-1.92 0.032-0.096 0.096-0.352 0.096-0.48 0.032-0.16 0.096-0.512 0.128-0.736 0.064-0.224 0.096-0.544 0.128-0.704 0-0.128 0.064-0.32 0.064-0.416 0.032-0.064 0.064-0.288 0.096-0.512 0.032-0.192 0.064-0.416 0.096-0.48 0-0.064 0.032-0.256 0.064-0.416s0.064-0.384 0.096-0.512c0.032-0.192 0.128-0.704 0.16-1.056 0.032-0.128 0.064-0.352 0.16-0.832 0.032-0.096 0.064-0.32 0.096-0.544 0.032-0.192 0.064-0.448 0.096-0.544 0.032-0.224 0.096-0.544 0.16-0.896 0.032-0.128 0.096-0.576 0.16-0.928 0.064-0.384 0.128-0.8 0.16-0.96s0.096-0.576 0.16-0.896c0.096-0.32 0.16-0.768 0.16-0.96 0.032-0.224 0.064-0.416 0.096-0.48 0.032-0.032 0.064-0.224 0.096-0.448 0-0.192 0.064-0.416 0.064-0.48 0.032-0.064 0.064-0.288 0.096-0.48 0-0.192 0.032-0.384 0.064-0.416 0.096-0.128 0.16-1.152 0.096-1.536-0.032-0.224-0.128-0.48-0.192-0.544-0.096-0.096-0.16-0.192-0.128-0.224 0.032 0-0.128-0.128-0.32-0.224-0.672-0.352-2.176-0.288-2.912 0.128-0.256 0.16-0.288 0.192-0.256 0.512 0.064 0.832 0.032 1.728-0.096 2.496-0.096 0.448-0.16 0.896-0.192 0.96 0 0.064-0.032 0.288-0.064 0.448-0.032 0.192-0.096 0.416-0.096 0.512-0.032 0.096-0.064 0.256-0.064 0.384-0.032 0.096-0.064 0.32-0.096 0.48s-0.128 0.8-0.256 1.376c-0.096 0.608-0.224 1.248-0.224 1.408-0.032 0.16-0.096 0.48-0.16 0.736-0.032 0.256-0.096 0.544-0.128 0.672 0 0.128-0.032 0.352-0.064 0.512s-0.16 0.768-0.256 1.376c-0.128 0.608-0.192 1.152-0.192 1.184 0 0.096-0.768 0.544-1.312 0.736-0.192 0.064-0.384 0.16-0.384 0.224s0 0.064-0.032 0.032-0.352 0.064-0.736 0.192c-1.632 0.544-3.008 0.608-3.488 0.128-0.192-0.192-0.192-0.256-0.192-0.928 0-0.736 0.032-0.896 0.992-4.448 0.064-0.256 0.096-0.512 0.064-0.512 0-0.032 0.032-0.096 0.064-0.096 0.032-0.032 0.096-0.16 0.128-0.288 0-0.128 0.032-0.256 0.032-0.256 0.032 0 0.064-0.128 0.128-0.48 0.096-0.48 0.096-0.512 0.128-0.544 0 0 0.032-0.032 0.032-0.064s0.064-0.224 0.128-0.448c0.064-0.192 0.128-0.448 0.128-0.544s0.032-0.224 0.064-0.288c0.48-1.344 0.48-3.2 0-4.256-0.352-0.8-1.216-1.408-2.208-1.6-0.416-0.064-1.696-0.096-1.76-0.032zM10.944 23.968c-0.032 0.192-0.128 0.416-0.16 0.544s-0.064 0.256-0.064 0.288c0 0.064 0 0.096-0.352 0.96-0.128 0.288-0.224 0.576-0.192 0.576 0.032 0.032 0 0.064-0.064 0.064s-0.224 0.32-0.192 0.448c0 0.032 0 0.032-0.032 0.032-0.064-0.032-0.16 0.064-0.224 0.224-0.192 0.288-0.608 0.704-0.832 0.768-0.064 0.032-0.128 0.064-0.128 0.096 0 0.096-0.064 0.096-0.704 0.128-0.544 0.032-0.736-0.064-0.96-0.512-0.16-0.224-0.128-0.992 0.032-1.408 0.064-0.16 0.128-0.352 0.128-0.416s0.032-0.096 0.064-0.064c0.064 0.032 0.096-0.032 0.128-0.128 0.064-0.192 0.832-0.928 0.992-0.928 0.032 0 0.032-0.032 0-0.064-0.032-0.064 0-0.096 0.032-0.096 0.096 0.064 0.704-0.256 0.8-0.384 0.032-0.032 0.064-0.032 0.064 0s0.064 0 0.16-0.032c0.16-0.096 1.28-0.416 1.472-0.416 0.064 0 0.064 0.096 0.032 0.32zM38.848 5.952c-0.16 0.032-0.384 0.064-0.512 0.096-0.288 0.064-1.44 0.48-1.504 0.576-0.032 0.064-0.064 0.064-0.064 0.032s-0.16 0.032-0.352 0.096c-0.32 0.192-0.576 0.224-0.544 0.128 0-0.128-0.128-0.352-0.256-0.352-0.064 0-0.096-0.032-0.096-0.064 0-0.16-0.608-0.352-1.312-0.384-0.48-0.064-2.048 0.384-1.92 0.512 0.032 0 0 0.096-0.032 0.128-0.064 0.096-0.064 0.224 0 0.448 0.096 0.416 0.096 1.248 0 1.632-0.064 0.16-0.096 0.416-0.128 0.64s-0.032 0.384-0.032 0.384c-0.032 0-0.064 0.16-0.128 0.576-0.032 0.16-0.064 0.384-0.096 0.48-0.032 0.128-0.064 0.32-0.064 0.48-0.032 0.16-0.064 0.384-0.096 0.512-0.064 0.224-0.448 2.496-0.512 2.816-0.032 0.256-0.096 0.576-0.192 1.184-0.064 0.256-0.128 0.608-0.128 0.768-0.032 0.128-0.064 0.384-0.096 0.48-0.288 1.6 0.032 2.368 1.056 2.592 0.48 0.128 1.728 0.032 1.888-0.096 0.032-0.032 0.128-0.064 0.224-0.064 0.064 0 0.128-0.032 0.128-0.096 0-0.032 0.032-0.064 0.064-0.064 0.352 0.064 0.448-0.224 0.32-0.8-0.128-0.544-0.096-0.896 0.096-1.856 0.064-0.416 0.16-0.864 0.16-0.992 0.032-0.128 0.064-0.352 0.096-0.448 0.096-0.544 0.128-0.64 0.16-0.896 0.032-0.128 0.064-0.352 0.064-0.48 0.032-0.16 0.064-0.384 0.096-0.512 0.224-1.152 0.288-1.568 0.256-1.632-0.032-0.032-0.032-0.096 0.032-0.128 0.032 0 0.064-0.128 0.064-0.256s0.064-0.48 0.128-0.736l0.096-0.512 0.576-0.256c0.64-0.32 0.992-0.416 1.44-0.32 0.544 0.096 0.704 0.704 0.512 1.824-0.032 0.192-0.096 0.416-0.096 0.512-0.032 0.096-0.064 0.256-0.064 0.384-0.032 0.096-0.064 0.32-0.096 0.48s-0.096 0.608-0.16 1.024c-0.064 0.384-0.16 0.832-0.16 1.024-0.032 0.16-0.064 0.32-0.096 0.384-0.032 0.032-0.064 0.224-0.096 0.48 0 0.224-0.064 0.48-0.096 0.608-0.224 1.152-0.288 2.112-0.16 2.56 0.128 0.32 0.608 0.8 0.736 0.768 0.064-0.032 0.192 0 0.32 0.064 0.256 0.16 1.376 0.096 1.984-0.096 0.576-0.16 0.8-0.384 0.736-0.672-0.032-0.128-0.096-0.32-0.096-0.448-0.032-0.128-0.064-0.256-0.064-0.288-0.032-0.064 0.032-0.512 0.128-1.024 0.064-0.512 0.16-1.056 0.192-1.216s0.096-0.448 0.128-0.704c0.096-0.448 0.16-0.896 0.192-1.152 0.032-0.096 0.096-0.544 0.16-0.96 0.096-0.448 0.16-0.896 0.192-0.992 0-0.128 0.064-0.352 0.064-0.512 0.032-0.16 0.128-0.544 0.16-0.864l0.096-0.576 0.544-0.288c0.768-0.384 1.344-0.48 1.664-0.288 0.16 0.096 0.32 0.288 0.352 0.416 0.096 0.256 0.032 1.088-0.128 1.984-0.064 0.288-0.096 0.448-0.288 1.664-0.224 1.312-0.256 1.472-0.32 1.792 0 0.16-0.032 0.352-0.064 0.416 0 0.064-0.064 0.256-0.064 0.384-0.032 0.16-0.096 0.416-0.096 0.544-0.224 1.216-0.224 1.76 0 2.24 0.128 0.224 0.288 0.352 0.576 0.512 0.384 0.192 0.512 0.192 1.216 0.192 0.608 0 0.896-0.032 1.28-0.192 0.608-0.224 0.672-0.352 0.544-0.928-0.096-0.512-0.032-1.408 0.192-2.464 0.032-0.224 0.096-0.576 0.128-0.736 0.032-0.192 0.096-0.608 0.16-0.928 0.064-0.288 0.096-0.576 0.096-0.608s0-0.064 0.032-0.096c0.032-0.096 0.064-0.288 0.096-0.672 0.032-0.224 0.096-0.448 0.096-0.512 0.032-0.064 0.064-0.256 0.096-0.416 0-0.16 0.064-0.384 0.064-0.448 0.032-0.128 0.064-0.32 0.096-0.48s0.064-0.352 0.064-0.448c0.224-1.088 0.32-2.272 0.192-2.848-0.096-0.512-0.128-0.576-0.256-0.832-0.416-0.8-1.12-1.184-2.432-1.248-0.608-0.032-2.464 0.448-2.464 0.64 0 0.064 0 0.064-0.032 0.032s-0.384 0.128-0.736 0.32l-0.704 0.352-0.16-0.224c-0.224-0.416-0.608-0.736-1.088-0.896-0.48-0.192-1.504-0.288-1.952-0.16zM21.536 6.048c0 0.032-0.224 0.064-0.48 0.064-0.544 0.064-1.184 0.224-1.184 0.352 0 0.032-0.032 0.032-0.064 0.032-0.032-0.032-0.128 0-0.224 0.096-0.128 0.16-0.128 0.192 0.032 0.832 0.064 0.224 0.032 0.864-0.064 1.376-0.064 0.288-0.128 0.608-0.128 0.768 0 0.128-0.064 0.416-0.128 0.64-0.032 0.224-0.096 0.544-0.128 0.704-0.064 0.544-0.096 0.704-0.16 0.864 0 0.064-0.064 0.32-0.064 0.544-0.032 0.224-0.064 0.416-0.096 0.448 0 0.032-0.064 0.224-0.096 0.48-0.032 0.224-0.064 0.48-0.064 0.544-0.032 0.064-0.064 0.256-0.096 0.416-0.096 0.544-0.128 0.8-0.16 1.024-0.16 0.896-0.096 2.208 0.096 2.624 0.064 0.096 0.128 0.256 0.192 0.384 0.16 0.352 0.704 0.896 1.056 1.024 0.928 0.384 1.664 0.416 2.784 0.128 0.224-0.064 0.416-0.128 0.448-0.128 0.064 0 0.16-0.064 0.256-0.096 0.704-0.288 1.472-0.544 1.504-0.512 0 0 0.064 0.128 0.128 0.256 0.288 0.608 0.896 0.864 1.888 0.864 0.64-0.032 1.536-0.256 1.632-0.416 0.032-0.032 0.096-0.064 0.128-0.096 0.032 0 0.064-0.16 0.064-0.384-0.096-1.248-0.096-1.472-0.032-1.76 0.032-0.16 0.096-0.416 0.128-0.576 0.064-0.576 0.128-0.96 0.16-1.12 0.032-0.096 0.064-0.288 0.096-0.448s0.064-0.384 0.096-0.48c0-0.096 0.032-0.288 0.064-0.448s0.096-0.576 0.16-0.896c0.064-0.288 0.128-0.576 0.096-0.608s0-0.096 0.032-0.16c0.032-0.096 0.096-0.32 0.128-0.512 0.032-0.224 0.064-0.48 0.096-0.608 0.032-0.192 0.32-1.792 0.416-2.272 0-0.16 0.064-0.352 0.064-0.48 0.128-0.448 0.064-1.312-0.096-1.632-0.128-0.288-0.736-0.768-0.832-0.672-0.032 0.032-0.096 0-0.16-0.032-0.096-0.096-1.088-0.128-1.44-0.032-0.448 0.096-1.056 0.32-1.184 0.416-0.096 0.096-0.096 0.192-0.032 0.544 0.096 0.448 0.096 1.312 0 1.824-0.032 0.16-0.128 0.576-0.192 0.928-0.064 0.32-0.096 0.64-0.096 0.64 0 0.032 0 0.096 0 0.128-0.032 0.064-0.096 0.352-0.128 0.576-0.032 0.192-0.128 0.704-0.192 1.024-0.032 0.096-0.064 0.32-0.064 0.48-0.032 0.16-0.064 0.32-0.064 0.384-0.032 0.032-0.064 0.256-0.096 0.48-0.064 0.224-0.096 0.448-0.096 0.48 0 0-0.064 0.32-0.128 0.704-0.096 0.576-0.128 0.64-0.352 0.736-0.128 0.064-0.224 0.128-0.192 0.128 0.032 0.032-0.032 0.064-0.096 0.064-0.096 0-0.32 0.064-0.512 0.16-0.864 0.32-1.856 0.064-1.92-0.512 0-0.096-0.032-0.224-0.032-0.288 0-0.16 0.16-1.472 0.192-1.472 0 0 0.032-0.064 0.032-0.16s0.032-0.288 0.064-0.416c0.032-0.128 0.096-0.384 0.096-0.512 0.128-0.704 0.192-1.152 0.256-1.44 0.032-0.128 0.064-0.384 0.096-0.544 0.032-0.192 0.128-0.8 0.256-1.344 0.288-1.632 0.16-2.432-0.416-2.784-0.16-0.064-0.288-0.16-0.352-0.16-0.512-0.096-0.864-0.16-0.896-0.16z"></path></svg></span>
									<span>Yummly</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-yahoo">
								<a href="#" data-ss-ss-link="https://compose.mail.yahoo.com/?body=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10&amp;subject=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010" data-id="yahoo" class="ss-yahoo-color" data-ss-ss-network-id="yahoo" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="27" height="32" viewBox="0 0 27 32" xmlns="http://www.w3.org/2000/svg"><path d="M15.339 17.375l0.232 12.625c-0.607-0.107-1.232-0.196-1.875-0.196-0.625 0-1.25 0.089-1.875 0.196l0.232-12.625c-3.321-5.732-6.446-11.571-10.107-17.089 0.625 0.161 1.268 0.268 1.929 0.268s1.339-0.125 1.982-0.268c2.5 4.429 5.214 8.732 7.839 13.089 2.643-4.321 5.446-8.625 7.839-13.089 0.625 0.161 1.268 0.25 1.911 0.25 0.679 0 1.375-0.089 2.036-0.25v0 0c-1.429 1.964-2.607 4.107-3.839 6.196-2.125 3.625-4.214 7.25-6.304 10.893z"></path></svg></span>
									<span>Yahoo</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-whatsapp">
								<a href="#" data-ss-ss-link="https://api.whatsapp.com/send?text=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010%20https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10" data-id="whatsapp" class="ss-whatsapp-color" data-ss-ss-network-id="whatsapp" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M27.313 4.625c-3-3-7-4.625-11.25-4.625-8.75 0-15.875 7.125-15.875 15.875 0 2.75 0.75 5.5 2.125 7.938l-2.25 8.188 8.438-2.188c2.313 1.25 4.875 1.938 7.563 1.938v0c0 0 0 0 0 0 8.75 0 15.875-7.125 15.875-15.875 0-4.25-1.625-8.25-4.625-11.25zM16.063 29.063v0c-2.375 0-4.688-0.625-6.688-1.875l-0.5-0.25-5 1.313 1.313-4.875-0.313-0.5c-1.313-2.125-2-4.5-2-7 0-7.313 5.938-13.188 13.188-13.188 3.5 0 6.813 1.375 9.313 3.875s3.875 5.813 3.875 9.313c0 7.25-5.938 13.188-13.188 13.188zM23.313 19.188c-0.438-0.188-2.375-1.188-2.75-1.313-0.313-0.125-0.625-0.188-0.875 0.188-0.25 0.438-1 1.313-1.25 1.563s-0.438 0.313-0.875 0.125c-0.375-0.188-1.625-0.625-3.188-2-1.125-1-1.938-2.313-2.188-2.75-0.25-0.375 0-0.563 0.188-0.813 0.188-0.125 0.375-0.438 0.563-0.688 0.25-0.188 0.313-0.375 0.438-0.625s0.063-0.5-0.063-0.688c-0.063-0.188-0.875-2.188-1.188-2.938-0.375-0.813-0.688-0.688-0.938-0.688-0.188 0-0.5 0-0.75 0s-0.688 0.063-1.063 0.438c-0.375 0.438-1.375 1.375-1.375 3.313 0 2 1.438 3.875 1.625 4.125s2.813 4.25 6.75 6c0.938 0.375 1.688 0.625 2.25 0.813 1 0.313 1.813 0.25 2.5 0.188 0.813-0.125 2.375-1 2.688-1.938 0.375-0.875 0.375-1.688 0.25-1.875-0.125-0.125-0.375-0.25-0.75-0.438z"></path></svg></span>
									<span>WhatsApp</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-viber">
								<a href="#" data-ss-ss-link="viber://forward?text=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010%20https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10" data-id="viber" class="ss-viber-color" data-ss-ss-network-id="viber" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M18.438 8.063c-0.375-0.063-0.75 0.25-0.75 0.688-0.063 0.375 0.25 0.75 0.688 0.813 2.5 0.125 3.688 1.375 3.813 4 0.063 0.375 0.375 0.688 0.813 0.688 0 0 0 0 0 0 0.438 0 0.75-0.375 0.75-0.75-0.188-3.438-2-5.25-5.313-5.438zM26.875 15.563c0.375 0 0.75-0.313 0.75-0.688 0.063-3-0.813-5.5-2.688-7.5-1.813-2-4.375-3.125-7.625-3.438-0.438 0-0.75 0.313-0.813 0.75 0 0.375 0.313 0.75 0.688 0.813 2.938 0.188 5.063 1.125 6.625 2.875 1.625 1.688 2.375 3.813 2.313 6.438 0 0.375 0.313 0.75 0.75 0.75zM27.063 4.438c-2.938-2.875-6.688-4.375-11.125-4.438-0.438 0-0.75 0.375-0.75 0.75 0 0.438 0.313 0.813 0.75 0.813 4 0 7.438 1.375 10.125 4s4.063 6.188 4.063 10.875c0 0.375 0.375 0.75 0.813 0.75 0.375 0 0.75-0.375 0.75-0.75-0.125-5.063-1.625-9.125-4.625-12zM29.875 25.063c0 0-1.75-1.438-2.625-2.063-0.813-0.625-2.063-1.375-2.75-1.813-1.313-0.688-2.625-0.25-3.125 0.5l-1.125 1.375c-0.625 0.688-1.688 0.625-1.688 0.625-7.813-2-9.875-9.938-9.875-9.938s-0.125-1.063 0.563-1.625l1.438-1.125c0.688-0.563 1.125-1.875 0.438-3.125-0.375-0.688-1.188-2-1.75-2.813-0.688-0.813-2.125-2.563-2.125-2.563-0.688-0.813-1.688-1-2.813-0.438 0 0 0 0 0 0-1.063 0.563-2 1.313-2.875 2.313 0 0 0 0 0 0.063-0.688 0.75-1.063 1.563-1.188 2.375 0 0.063 0 0.188 0 0.313 0 0.375 0 0.688 0.125 1.063h0.063c0.313 1.188 1.188 3.188 3 6.563 1.188 2.125 2.375 3.938 3.625 5.438 0.625 0.813 1.313 1.625 2.188 2.438 0 0.063 0.063 0.125 0.063 0.125 0.063 0.063 0.063 0.063 0.125 0.125 0 0 0.063 0.063 0.063 0.063 0.063 0.063 0.063 0.063 0.125 0.125 0.813 0.813 1.625 1.5 2.438 2.125 1.5 1.25 3.313 2.438 5.5 3.625 3.313 1.875 5.313 2.688 6.5 3l0.063 0.063c0.313 0.063 0.625 0.188 1 0.188 0.125 0 0.25 0 0.375-0.063 0.75-0.125 1.563-0.5 2.313-1.125 0 0 0 0 0.063-0.063 1-0.875 1.75-1.875 2.313-2.875 0 0 0 0 0-0.063 0.563-1.063 0.375-2.063-0.438-2.813z"></path></svg></span>
									<span>Viber</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-sms">
								<a href="#" data-ss-ss-link="sms:?&amp;body=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010%20https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10" data-id="sms" class="ss-sms-color" data-ss-ss-network-id="sms" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M24 10.688v-2.688h-16v2.688h16zM18.688 18.688v-2.688h-10.688v2.688h10.688zM8 12v2.688h16v-2.688h-16zM26.688 2.688c1.438 0 2.625 1.188 2.625 2.625v16c0 1.438-1.188 2.688-2.625 2.688h-18.688l-5.313 5.313v-24c0-1.438 1.188-2.625 2.625-2.625h21.375z"></path></svg></span>
									<span>SMS</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-telegram">
								<a href="#" data-ss-ss-link="https://t.me/share/url?url=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010%20https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10" data-id="telegram" class="ss-telegram-color" data-ss-ss-network-id="telegram" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="28" height="32" viewBox="0 0 28 32" xmlns="http://www.w3.org/2000/svg"><path d="M27.919 6.162l-4.225 19.925c-0.319 1.406-1.15 1.756-2.331 1.094l-6.438-4.744-3.106 2.988c-0.344 0.344-0.631 0.631-1.294 0.631l0.463-6.556 11.931-10.781c0.519-0.463-0.113-0.719-0.806-0.256l-14.75 9.287-6.35-1.988c-1.381-0.431-1.406-1.381 0.288-2.044l24.837-9.569c1.15-0.431 2.156 0.256 1.781 2.013z"></path></svg></span>
									<span>Telegram</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-messenger">
								<a href="#" data-ss-ss-link="https://www.facebook.com/dialog/send?display=popup&amp;link=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10&amp;app_id=772401629609127&amp;redirect_uri=https://www.thewindowsclub.com/" data-id="messenger" class="ss-messenger-color" data-ss-ss-network-id="messenger" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M16 0c-8.768 0-15.904 6.624-15.904 14.816 0 4.672 2.304 8.832 5.92 11.552v5.632l5.408-2.976c1.44 0.416 2.976 0.608 4.576 0.608 8.768 0 15.904-6.624 15.904-14.816s-7.136-14.816-15.904-14.816zM17.568 19.936l-4.032-4.32-7.904 4.32 8.704-9.28 4.16 4.352 7.808-4.352-8.736 9.28z"></path></svg></span>
									<span>Facebook Messenger</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-heart">
								<a href="#" data-ss-ss-link="#" data-id="heart" class="ss-heart-color" data-ss-ss-network-id="heart" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="like" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M16 30c-0.286 0-0.571-0.107-0.786-0.321l-11.143-10.75c-0.143-0.125-4.071-3.714-4.071-8 0-5.232 3.196-8.357 8.536-8.357 3.125 0 6.054 2.464 7.464 3.857 1.411-1.393 4.339-3.857 7.464-3.857 5.339 0 8.536 3.125 8.536 8.357 0 4.286-3.929 7.875-4.089 8.036l-11.125 10.714c-0.214 0.214-0.5 0.321-0.786 0.321z"></path></svg></span>
									<span>Like</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-envelope">
								<a href="#" data-ss-ss-link="mailto:?body=https%3A%2F%2Fwww.thewindowsclub.com%2Fhow-to-run-sh-or-shell-script-file-in-windows-10&amp;subject=How%20to%20run%20.sh%20or%20Shell%20Script%20file%20in%20Windows%2010" data-id="envelope" class="ss-envelope-color" data-ss-ss-network-id="envelope" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M32 12.964v14.179c0 1.571-1.286 2.857-2.857 2.857h-26.286c-1.571 0-2.857-1.286-2.857-2.857v-14.179c0.536 0.589 1.143 1.107 1.804 1.554 2.964 2.018 5.964 4.036 8.875 6.161 1.5 1.107 3.357 2.464 5.304 2.464h0.036c1.946 0 3.804-1.357 5.304-2.464 2.911-2.107 5.911-4.143 8.893-6.161 0.643-0.446 1.25-0.964 1.786-1.554zM32 7.714c0 2-1.482 3.804-3.054 4.893-2.786 1.929-5.589 3.857-8.357 5.804-1.161 0.804-3.125 2.446-4.571 2.446h-0.036c-1.446 0-3.411-1.643-4.571-2.446-2.768-1.946-5.571-3.875-8.339-5.804-1.268-0.857-3.071-2.875-3.071-4.5 0-1.75 0.946-3.25 2.857-3.25h26.286c1.554 0 2.857 1.286 2.857 2.857z"></path></svg></span>
									<span>Email</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-print">
								<a href="#" data-ss-ss-link="#" data-id="print" class="ss-print-color" data-ss-ss-network-id="print" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="30" height="32" viewBox="0 0 30 32" xmlns="http://www.w3.org/2000/svg"><path d="M6.857 27.714h16v-4.571h-16v4.571zM6.857 16.286h16v-6.857h-2.857c-0.946 0-1.714-0.768-1.714-1.714v-2.857h-11.429v11.429zM27.429 17.429c0-0.625-0.518-1.143-1.143-1.143s-1.143 0.518-1.143 1.143 0.518 1.143 1.143 1.143 1.143-0.518 1.143-1.143zM29.714 17.429v7.429c0 0.304-0.268 0.571-0.571 0.571h-4v2.857c0 0.946-0.768 1.714-1.714 1.714h-17.143c-0.946 0-1.714-0.768-1.714-1.714v-2.857h-4c-0.304 0-0.571-0.268-0.571-0.571v-7.429c0-1.875 1.554-3.429 3.429-3.429h1.143v-9.714c0-0.946 0.768-1.714 1.714-1.714h12c0.946 0 2.25 0.536 2.929 1.214l2.714 2.714c0.679 0.679 1.214 1.982 1.214 2.929v4.571h1.143c1.875 0 3.429 1.554 3.429 3.429z"></path></svg></span>
									<span>Print</span>
								</a>
							</div>

						
							<div class="ss-popup-network ss-popup-copy">
								<a href="#" data-ss-ss-link="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-id="copy" class="ss-copy-color" data-ss-ss-network-id="copy" data-ss-ss-post-id="186120" data-ss-ss-location="popup" data-ss-ss-permalink="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" data-ss-ss-type="share" rel="nofollow noopener">
									<span><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M25.313 28v-18.688h-14.625v18.688h14.625zM25.313 6.688c1.438 0 2.688 1.188 2.688 2.625v18.688c0 1.438-1.25 2.688-2.688 2.688h-14.625c-1.438 0-2.688-1.25-2.688-2.688v-18.688c0-1.438 1.25-2.625 2.688-2.625h14.625zM21.313 1.313v2.688h-16v18.688h-2.625v-18.688c0-1.438 1.188-2.688 2.625-2.688h16z"></path></svg></span>
									<span>Copy Link</span>
								</a>
							</div>

											</div><!-- END .ss-popup-networks -->

					<div class="ss-powered-by">Powered by <a href="https://socialsnap.com/?utm_source=WordPress&amp;utm_medium=link&amp;utm_campaign=inthewild" target="_blank" rel="nofollow noopener"><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="30" height="32" viewBox="0 0 30 32" xmlns="http://www.w3.org/2000/svg"><path d="M22.293 0.146l7.602 4.172c0.386 0.201 0.386 0.541 0 0.757l-16.688 9.147c-1.684 0.943-2.241 2.271-1.669 3.461 0 0.093 0 0.201-0.201 0.263-0.207 0.088-0.441 0.088-0.649 0l-10.399-5.702c-0.386-0.201-0.386-0.541 0-0.757l20.628-11.311c0.428-0.225 0.937-0.236 1.375-0.031zM7.892 31.854l-7.602-4.172c-0.386-0.201-0.386-0.541 0-0.757l16.688-9.147c1.684-0.943 2.241-2.271 1.669-3.461 0-0.093 0-0.201 0.201-0.263 0.207-0.088 0.442-0.088 0.649 0l10.399 5.702c0.386 0.201 0.386 0.541 0 0.757l-20.628 11.311c-0.428 0.225-0.937 0.237-1.375 0.031z"></path></svg>Social Snap</a></div><!-- END .ss-powered-by -->
				</div><!-- END .ss-popup-content -->
			</div><!-- END .ss-popup -->
		</div><!-- END #ss-all-networks-popup -->

		
		<div id="ss-copy-popup" class="ss-popup-overlay">
			<div class="ss-popup">

				<div class="ss-popup-heading">
					<span>Copy link</span>
					<a href="#" class="ss-close-modal" rel="nofollow noopener">
						<svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M17.883 16.667l7.058-7.058c0.517-0.517 0.517-1.367 0-1.883s-1.367-0.517-1.883 0l-7.058 7.058-7.058-7.058c-0.517-0.517-1.367-0.517-1.883 0s-0.517 1.367 0 1.883l7.058 7.058-7.058 7.058c-0.517 0.517-0.517 1.367 0 1.883 0.258 0.258 0.6 0.392 0.942 0.392s0.683-0.133 0.942-0.392l7.058-7.058 7.058 7.058c0.258 0.258 0.6 0.392 0.942 0.392s0.683-0.133 0.942-0.392c0.517-0.517 0.517-1.367 0-1.883l-7.058-7.058z"></path></svg>					</a>
				</div><!-- END .ss-popup-heading -->

				<div class="ss-popup-content">

					<div class="ss-copy-action">
						<input type="text" readonly="readonly" value="https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10" class="ss-copy-action-field" aria-label="Copy"/>
						<a href="#" class="ss-button" rel="nofollow noopener">Copy<span class="ss-share-network-tooltip">Copied</span></a>
						<svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M25.313 28v-18.688h-14.625v18.688h14.625zM25.313 6.688c1.438 0 2.688 1.188 2.688 2.625v18.688c0 1.438-1.25 2.688-2.688 2.688h-14.625c-1.438 0-2.688-1.25-2.688-2.688v-18.688c0-1.438 1.25-2.625 2.688-2.625h14.625zM21.313 1.313v2.688h-16v18.688h-2.625v-18.688c0-1.438 1.188-2.688 2.625-2.688h16z"></path></svg>					</div><!-- END .ss-copy-action -->

					<div class="ss-powered-by">Powered by <a href="https://socialsnap.com/?utm_source=WordPress&amp;utm_medium=link&amp;utm_campaign=inthewild" target="_blank" rel="nofollow noopener"><svg class="ss-svg-icon" aria-hidden="true" role="img" focusable="false" width="30" height="32" viewBox="0 0 30 32" xmlns="http://www.w3.org/2000/svg"><path d="M22.293 0.146l7.602 4.172c0.386 0.201 0.386 0.541 0 0.757l-16.688 9.147c-1.684 0.943-2.241 2.271-1.669 3.461 0 0.093 0 0.201-0.201 0.263-0.207 0.088-0.441 0.088-0.649 0l-10.399-5.702c-0.386-0.201-0.386-0.541 0-0.757l20.628-11.311c0.428-0.225 0.937-0.236 1.375-0.031zM7.892 31.854l-7.602-4.172c-0.386-0.201-0.386-0.541 0-0.757l16.688-9.147c1.684-0.943 2.241-2.271 1.669-3.461 0-0.093 0-0.201 0.201-0.263 0.207-0.088 0.442-0.088 0.649 0l10.399 5.702c0.386 0.201 0.386 0.541 0 0.757l-20.628 11.311c-0.428 0.225-0.937 0.237-1.375 0.031z"></path></svg>Social Snap</a></div><!-- END .ss-powered-by -->
				</div><!-- END .ss-popup-content -->
			</div><!-- END .ss-popup -->
		</div><!-- END #ss-copy-popup -->

				<!-- Social Snap Share count cache indicator -->
		<script type="text/javascript">

			var SocialSnapURL 				= window.location.href;
			var SocialSnapShareCacheExpired = 0;
			var SocialSnapShareNetworks     = ["facebook","twitter","linkedin","reddit","whatsapp","mix","pinterest","tumblr","skype","buffer","pocket","vkontakte","parler","xing","flipboard","myspace","delicious","amazon","digg","evernote","blogger","livejournal","baidu","mewe","newsvine","yummly","yahoo","viber","sms","telegram","messenger","heart","envelope","print","copy"];

			if ( -1 !== SocialSnapURL.indexOf('ss_cache_refresh') ) {

				SocialSnapShareCacheExpired = true;

			} else {

				var SocialSnapServerTimestamp 	= 1614883424;
				var SocialSnapBrowserTimestamp 	= Date.now();

				if ( ! SocialSnapBrowserTimestamp ) {
					SocialSnapBrowserTimestamp = new Date().getTime();
				}

				SocialSnapBrowserTimestamp = Math.floor( SocialSnapBrowserTimestamp / 1000 );

				SocialSnapShareCacheExpired = SocialSnapShareCacheExpired && ( SocialSnapBrowserTimestamp - SocialSnapServerTimestamp < 60 );
			}

		</script>
		<!-- Social Snap Share count cache indicator -->
		

<script type="text/javascript">
				var __inScopeForCCPA = false;
		function __uspapi(command, version, callback) {
			var response = null;
			var successs = false;
			if (command === "getUSPData" && version === 1) {
				var uspString = "1"; // Version
				if (__inScopeForCCPA) {
					uspString += "Y"; // Has Explicit Notice for Opt Out been provided (ex footer or minor consent modal)
					var result;
					var consentCookie = (result = new RegExp('(?:^|; )ezoccpaconsent=([^;]*)').exec(document.cookie)) ? (result[1]) : null;
					if (consentCookie === "nonconsent") {
						uspString += "Y";
					}
					else {
						uspString += "N";
					}
					uspString += "N" // Is pub a signatory to the IAB Limited Service Provider Agreement (http://www.iabprivacy.com/)
				}
				else {
					uspString += "---";
				}
				response = {
					uspString: uspString,
					version: 1
				};
				success = true;
			}
			return callback(response, success);
		};
		function __receiveUspapiMessage(event) {
			if (event.data.hasOwnProperty('__uspapiCall')) {
				__uspapi('getUSPData', 1, function(uspData, success) {
					event.source.postMessage({
						__uspapiReturn: {
							returnValue: uspData,
							success: success,
							callId: event.data.__uspapiCall.callId
						}
					},
					event.origin);
				});
			}
			return null;
		};
		window.addEventListener("message", __receiveUspapiMessage, false);
</script>
<script>var __ez_tkn_evnt = function() { if(typeof(_ezaq) != 'undefined'){if(window.ezogtk != "") {__ez.bit.AddAndFire(_ezaq.page_view_id,[new __ezDotData("ext_user_hash",window.ezogtk)]);}}};document.addEventListener("DOMContentLoaded", __ez.queue.addFunc("__ez_tkn_evnt", "__ez_tkn_evnt", event, false, ['/detroitchicago/minneapolis.js','/detroitchicago/memphis.js'], true, true, false, true));</script>
<script src="/detroitchicago/augusta.js?cb=3" async data-ezscrex="false"></script>
<script type="text/javascript">(function(f,a){function g(b,a,c){b.addEventListener?b.addEventListener(a,c):b.attachEvent("on"+a,function(){c.call(b)})}function k(b){b&&("string"==typeof b["class"]&&b["class"]&&a.getElementById("uglipop_popbox").setAttribute("class",b["class"]),b.keepLayout&&!b["class"]&&a.getElementById("uglipop_popbox").setAttribute("style","position:relative;height:300px;width:300px;background-color:white;opacity:1;"),"string"==typeof b.content&&b.content&&"html"==b.source&&(a.getElementById("uglipop_popbox").innerHTML=b.content),"string"==typeof b.content&&b.content&&"div"==b.source&&(a.getElementById("uglipop_popbox").innerHTML=a.getElementById(b.content).innerHTML));a.getElementById("uglipop_overlay_wrapper").style.display="";a.getElementById("uglipop_overlay").style.display="";a.getElementById("uglipop_content_fixed").style.display=""}function h(){a.getElementById("uglipop_overlay_wrapper").style.display="none";a.getElementById("uglipop_overlay").style.display="none";a.getElementById("uglipop_content_fixed").style.display="none"}g(a,"DOMContentLoaded",function(){var b=a.createElement("div"),e=a.createElement("div"),c=a.createElement("div"),d=a.createElement("div");e.id="uglipop_content_fixed";e.setAttribute("style","position:fixed;top: 50%;left: 50%;transform: translate(-50%, -50%);-webkit-transform: translate(-50%, -50%);-ms-transform: translate(-50%, -50%);opacity:1;z-index:10000000;");c.id="uglipop_popbox";d.id="uglipop_overlay_wrapper";d.setAttribute("style","position:absolute;top:0;bottom:0;left:0;right:0;display:none");b.id="uglipop_overlay";b.setAttribute("style","position:fixed;top:0;bottom:0;left:0;right:0;opacity:0.3;width:100%;height:100%;background-color:black;");d.appendChild(b);e.appendChild(c);a.body.appendChild(d);a.body.appendChild(e);a.getElementById("uglipop_overlay_wrapper").style.display="none";a.getElementById("uglipop_overlay").style.display="none";a.getElementById("uglipop_content_fixed").style.display="none";d.addEventListener("click",h);g(f,"keydown",function(a){27==a.keyCode&&h()});f.uglipop=k})})(window,document);var ezRBA=(function(){function init(){var reportAdsBtns=document.querySelectorAll('.ez-report-ad-button');for(var i=0;i<reportAdsBtns.length;i++){reportAdsBtns[i].addEventListener('click',function(e){var url='<iframe src="https://svc.ezoic.com/pub/reportads/reportads.html'+e.target.getAttribute('name')+'" width="400" height="500" style="border-radius: 10px; box-shadow: 2px 2px 30px 6px rgba(0,0,0,0.75); border: 1px solid black;"></iframe>'
uglipop({class:'none',source:'html',content:url,});});}
function bindEvent(element,eventName,eventHandler){if(element.addEventListener){element.addEventListener(eventName,eventHandler,false);}else if(element.attachEvent){element.attachEvent('on'+eventName,eventHandler);}}
bindEvent(window,'message',function(e){if(e.data==='close-report-ad-modal'){document.getElementById('uglipop_overlay_wrapper').style.display='none';document.getElementById('uglipop_overlay').style.display='none';document.getElementById('uglipop_content_fixed').style.display='none';}})}
return{init:init};})();ezRBA.init();</script>
<script type="text/javascript" data-cfasync="false"></script>
<script data-ezscrex='false' data-pagespeed-no-defer data-cfasync='false' type='text/javascript' style='display:none'>
__ez_func_ezosuigeneris = function() { if(typeof ezosuigeneris != "undefined") { var ezosuigenerisDate = new Date(); ezosuigenerisDate.setMonth(ezosuigenerisDate.getMonth() + 24); __ez.ck.setByCat("ezosuigeneris=" + window.ezosuigeneris + ";expires=" + ezosuigenerisDate.toUTCString() + ";domain="+window.ezdomain+";path=/",3); } };
__ez.queue.addFunc('__ez_func_ezosuigeneris', '__ez_func_ezosuigeneris', null, false, ['__ezf_ezosuigeneris','/detroitchicago/boise.js'], true, false, false, false);

__ez_func_ezosuigenerisc = function() { if(typeof ezosuigenerisc != "undefined") { var ezosuigeneriscDate = new Date(); ezosuigeneriscDate.setMonth(ezosuigeneriscDate.getMonth() + 24); __ez.ck.setByCat("ezosuigenerisc=" + window.ezosuigenerisc + ";expires=" + ezosuigeneriscDate.toUTCString() + ";domain="+window.ezdomain+";path=/",3); } };
__ez.queue.addFunc('__ez_func_ezosuigenerisc', '__ez_func_ezosuigenerisc', null, false, ['__ezf_ezosuigenerisc','/detroitchicago/boise.js'], true, false, false, false);
</script>
<script type="text/javascript" style='display:none;'>var __ez_dims = (function() {
		var setCookie = function( name, content, expiry ) {
			return document.cookie = name+'='+content+((expiry)?';expires='+(new Date(Math.floor(new Date().getTime()+expiry*1000)).toUTCString()):'')+';path=/';
		};
		var ffid = 1;
		var oh = window.screen.height;
		var ow = window.screen.width;
		var h = ffid === 1 ? oh : (oh > ow) ? oh : ow;
		var w = ffid === 1 ? ow : (oh > ow) ? ow : oh;
		var uh = window.innerHeight || document.documentElement.clientHeight || document.getElementsByTagName('body')[0].clientHeight;
		var uw = window.innerWidth || document.documentElement.clientWidth || document.getElementsByTagName('body')[0].clientWidth;
		setCookie('ezds', encodeURIComponent('ffid='+ffid+',w='+w+',h='+h), (31536e3*7));
		setCookie('ezohw', encodeURIComponent('w='+uw+',h='+uh), (31536e3*7));
	})();</script><script type='text/javascript' style='display:none;' async>
__ez.queue.addFile('edmonton.php', '/detroitchicago/edmonton.webp?a=a&cb=192-3&shcb=34', true, ['/detroitchicago/minneapolis.js'], true, false, false, false);
__ez.queue.addFile('jellyfish.php', '/porpoiseant/jellyfish.webp?a=a&cb=192-3&shcb=34', false, [], true, false, false, false);
</script>

<script>var _audins_dom="thewindowsclub_com",_audins_did=77472;__ez.queue.addDelayFunc("audins.js","__ez.script.add", "//go.ezoic.net/detroitchicago/audins.js?cb=192-3");</script><noscript><div style="display:none;"><img src="//pixel.quantserve.com/pixel/p-31iz6hfFutd16.gif?labels=Domain.thewindowsclub_com,DomainId.77472" border="0" height="1" width="1" alt="Quantcast"/></div></noscript>
<script>__ez.queue.addFile('/tardisrocinante/vitals.js', '/tardisrocinante/vitals.js?gcb=3&cb=3', false, ['/detroitchicago/minneapolis.js'], true, false, true, false);</script></body></html>
