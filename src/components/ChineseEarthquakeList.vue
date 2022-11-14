<template>
    <div>
        <div id="mainBar">
			<div id="mainLeft">
				<div id="mainTime">{{mainTime}}</div>
				<div id="mainEpicenter">{{mainEpicenter}}</div>
				<div id="mainDepth">{{mainDepth}}<font size="3">&nbsp;km</font></div>
				<div id="mainMagnitude"><font size="4">M</font>{{mainMagnitude}}</div>
			</div>
			<div id="mainMaxInt" :style="{'background-color':mainMaxIntColor}"><span style="position:relative; top:-2px;">{{mainMaxInt}}</span></div>
		</div>
		<div id="subBar2">
			<div id="subLeft2">
				<div id="subTime2">{{subTime[2]}}</div>
				<div id="subEpicenter2" :style="{'font-size':subEpicenterFontSize[2]}">{{subEpicenter[2]}}</div>
				<div id="subMagnitude2">M{{subMagnitude[2]}}</div>
			</div>
			<div id="subMaxInt2" :style="{'background-color':subMaxIntColor[2]}"><span style="position:relative; top:-2px;">{{subMaxInt[2]}}</span></div>
		</div>
        <div id=subBar3><div id=subLeft3><div id=subTime3>{{subTime[3]}}</div><div id=subEpicenter3 :style="{'font-size':subEpicenterFontSize[3]}">{{subEpicenter[3]}}</div><div id=subMagnitude3>M{{subMagnitude[3]}}</div></div><div id=subMaxInt3 :style="{'background-color':subMaxIntColor[3]}"><span style="position:relative; top:-2px;">{{subMaxInt[3]}}</span></div></div>
        <div id=subBar3><div id=subLeft4><div id=subTime4>{{subTime[4]}}</div><div id=subEpicenter4 :style="{'font-size':subEpicenterFontSize[4]}">{{subEpicenter[4]}}</div><div id=subMagnitude4>M{{subMagnitude[4]}}</div></div><div id=subMaxInt4 :style="{'background-color':subMaxIntColor[4]}"><span style="position:relative; top:-2px;">{{subMaxInt[4]}}</span></div></div>
        <div id=subBar5><div id=subLeft5><div id=subTime5>{{subTime[5]}}</div><div id=subEpicenter5 :style="{'font-size':subEpicenterFontSize[5]}">{{subEpicenter[5]}}</div><div id=subMagnitude5>M{{subMagnitude[5]}}</div></div><div id=subMaxInt5 :style="{'background-color':subMaxIntColor[5]}"><span style="position:relative; top:-2px;">{{subMaxInt[5]}}</span></div></div>
        <div id=subBar6><div id=subLeft6><div id=subTime6>{{subTime[6]}}</div><div id=subEpicenter6 :style="{'font-size':subEpicenterFontSize[6]}">{{subEpicenter[6]}}</div><div id=subMagnitude6>M{{subMagnitude[6]}}</div></div><div id=subMaxInt6 :style="{'background-color':subMaxIntColor[6]}"><span style="position:relative; top:-2px;">{{subMaxInt[6]}}</span></div></div>
        <div id=subBar7><div id=subLeft7><div id=subTime7>{{subTime[7]}}</div><div id=subEpicenter7 :style="{'font-size':subEpicenterFontSize[7]}">{{subEpicenter[7]}}</div><div id=subMagnitude7>M{{subMagnitude[7]}}</div></div><div id=subMaxInt7 :style="{'background-color':subMaxIntColor[7]}"><span style="position:relative; top:-2px;">{{subMaxInt[7]}}</span></div></div>
        <div id=subBar8><div id=subLeft8><div id=subTime8>{{subTime[8]}}</div><div id=subEpicenter8 :style="{'font-size':subEpicenterFontSize[8]}">{{subEpicenter[8]}}</div><div id=subMagnitude8>M{{subMagnitude[8]}}</div></div><div id=subMaxInt8 :style="{'background-color':subMaxIntColor[8]}"><span style="position:relative; top:-2px;">{{subMaxInt[8]}}</span></div></div>
        <div id=subBar9><div id=subLeft9><div id=subTime9>{{subTime[9]}}</div><div id=subEpicenter9 :style="{'font-size':subEpicenterFontSize[9]}">{{subEpicenter[9]}}</div><div id=subMagnitude9>M{{subMagnitude[9]}}</div></div><div id=subMaxInt9 :style="{'background-color':subMaxIntColor[9]}"><span style="position:relative; top:-2px;">{{subMaxInt[9]}}</span></div></div>
        <div id=subBar10><div id=subLeft10><div id=subTime10>{{subTime[10]}}</div><div id=subEpicenter10 :style="{'font-size':subEpicenterFontSize[10]}">{{subEpicenter[10]}}</div><div id=subMagnitude10>M{{subMagnitude[10]}}</div></div><div id=subMaxInt10 :style="{'background-color':subMaxIntColor[10]}"><span style="position:relative; top:-2px;">{{subMaxInt[10]}}</span></div></div>
        <div id=subBar11><div id=subLeft11><div id=subTime11>{{subTime[11]}}</div><div id=subEpicenter11 :style="{'font-size':subEpicenterFontSize[11]}">{{subEpicenter[11]}}</div><div id=subMagnitude11>M{{subMagnitude[11]}}</div></div><div id=subMaxInt11 :style="{'background-color':subMaxIntColor[11]}"><span style="position:relative; top:-2px;">{{subMaxInt[11]}}</span></div></div>
        <div id=subBar12><div id=subLeft12><div id=subTime12>{{subTime[12]}}</div><div id=subEpicenter12 :style="{'font-size':subEpicenterFontSize[12]}">{{subEpicenter[12]}}</div><div id=subMagnitude12>M{{subMagnitude[12]}}</div></div><div id=subMaxInt12 :style="{'background-color':subMaxIntColor[12]}"><span style="position:relative; top:-2px;">{{subMaxInt[12]}}</span></div></div>
        <div id=subBar13><div id=subLeft13><div id=subTime13>{{subTime[13]}}</div><div id=subEpicenter13 :style="{'font-size':subEpicenterFontSize[13]}">{{subEpicenter[13]}}</div><div id=subMagnitude13>M{{subMagnitude[13]}}</div></div><div id=subMaxInt13 :style="{'background-color':subMaxIntColor[13]}"><span style="position:relative; top:-2px;">{{subMaxInt[13]}}</span></div></div>
        <div id=subBar14><div id=subLeft14><div id=subTime14>{{subTime[14]}}</div><div id=subEpicenter14 :style="{'font-size':subEpicenterFontSize[14]}">{{subEpicenter[14]}}</div><div id=subMagnitude14>M{{subMagnitude[14]}}</div></div><div id=subMaxInt14 :style="{'background-color':subMaxIntColor[14]}"><span style="position:relative; top:-2px;">{{subMaxInt[14]}}</span></div></div>
        <div id=subBar15><div id=subLeft15><div id=subTime15>{{subTime[15]}}</div><div id=subEpicenter15 :style="{'font-size':subEpicenterFontSize[15]}">{{subEpicenter[15]}}</div><div id=subMagnitude15>M{{subMagnitude[15]}}</div></div><div id=subMaxInt15 :style="{'background-color':subMaxIntColor[15]}"><span style="position:relative; top:-2px;">{{subMaxInt[15]}}</span></div></div>
        <div id=subBar16><div id=subLeft16><div id=subTime16>{{subTime[16]}}</div><div id=subEpicenter16 :style="{'font-size':subEpicenterFontSize[16]}">{{subEpicenter[16]}}</div><div id=subMagnitude16>M{{subMagnitude[16]}}</div></div><div id=subMaxInt16 :style="{'background-color':subMaxIntColor[16]}"><span style="position:relative; top:-2px;">{{subMaxInt[16]}}</span></div></div>
        <div id=subBar17><div id=subLeft17><div id=subTime17>{{subTime[17]}}</div><div id=subEpicenter17 :style="{'font-size':subEpicenterFontSize[17]}">{{subEpicenter[17]}}</div><div id=subMagnitude17>M{{subMagnitude[17]}}</div></div><div id=subMaxInt17 :style="{'background-color':subMaxIntColor[17]}"><span style="position:relative; top:-2px;">{{subMaxInt[17]}}</span></div></div>
        <div id=subBar18><div id=subLeft18><div id=subTime18>{{subTime[18]}}</div><div id=subEpicenter18 :style="{'font-size':subEpicenterFontSize[18]}">{{subEpicenter[18]}}</div><div id=subMagnitude18>M{{subMagnitude[18]}}</div></div><div id=subMaxInt18 :style="{'background-color':subMaxIntColor[18]}"><span style="position:relative; top:-2px;">{{subMaxInt[18]}}</span></div></div>
        <div id=subBar19><div id=subLeft19><div id=subTime19>{{subTime[19]}}</div><div id=subEpicenter19 :style="{'font-size':subEpicenterFontSize[19]}">{{subEpicenter[19]}}</div><div id=subMagnitude19>M{{subMagnitude[19]}}</div></div><div id=subMaxInt19 :style="{'background-color':subMaxIntColor[19]}"><span style="position:relative; top:-2px;">{{subMaxInt[19]}}</span></div></div>
        <div id=subBar20><div id=subLeft20><div id=subTime20>{{subTime[20]}}</div><div id=subEpicenter20 :style="{'font-size':subEpicenterFontSize[20]}">{{subEpicenter[20]}}</div><div id=subMagnitude20>M{{subMagnitude[20]}}</div></div><div id=subMaxInt20 :style="{'background-color':subMaxIntColor[20]}"><span style="position:relative; top:-2px;">{{subMaxInt[20]}}</span></div></div>
        <div id=subBar21><div id=subLeft21><div id=subTime21>{{subTime[21]}}</div><div id=subEpicenter21 :style="{'font-size':subEpicenterFontSize[21]}">{{subEpicenter[21]}}</div><div id=subMagnitude21>M{{subMagnitude[21]}}</div></div><div id=subMaxInt21 :style="{'background-color':subMaxIntColor[21]}"><span style="position:relative; top:-2px;">{{subMaxInt[21]}}</span></div></div>
        <div id=subBar22><div id=subLeft22><div id=subTime22>{{subTime[22]}}</div><div id=subEpicenter22 :style="{'font-size':subEpicenterFontSize[22]}">{{subEpicenter[22]}}</div><div id=subMagnitude22>M{{subMagnitude[22]}}</div></div><div id=subMaxInt22 :style="{'background-color':subMaxIntColor[22]}"><span style="position:relative; top:-2px;">{{subMaxInt[22]}}</span></div></div>
        <div id=subBar23><div id=subLeft23><div id=subTime23>{{subTime[23]}}</div><div id=subEpicenter23 :style="{'font-size':subEpicenterFontSize[23]}">{{subEpicenter[23]}}</div><div id=subMagnitude23>M{{subMagnitude[23]}}</div></div><div id=subMaxInt23 :style="{'background-color':subMaxIntColor[23]}"><span style="position:relative; top:-2px;">{{subMaxInt[23]}}</span></div></div>
        <div id=subBar24><div id=subLeft24><div id=subTime24>{{subTime[24]}}</div><div id=subEpicenter24 :style="{'font-size':subEpicenterFontSize[24]}">{{subEpicenter[24]}}</div><div id=subMagnitude24>M{{subMagnitude[24]}}</div></div><div id=subMaxInt24 :style="{'background-color':subMaxIntColor[24]}"><span style="position:relative; top:-2px;">{{subMaxInt[24]}}</span></div></div>
        <div id=subBar25><div id=subLeft25><div id=subTime25>{{subTime[25]}}</div><div id=subEpicenter25 :style="{'font-size':subEpicenterFontSize[25]}">{{subEpicenter[25]}}</div><div id=subMagnitude25>M{{subMagnitude[25]}}</div></div><div id=subMaxInt25 :style="{'background-color':subMaxIntColor[25]}"><span style="position:relative; top:-2px;">{{subMaxInt[25]}}</span></div></div>
        <div id=subBar26><div id=subLeft26><div id=subTime26>{{subTime[26]}}</div><div id=subEpicenter26 :style="{'font-size':subEpicenterFontSize[26]}">{{subEpicenter[26]}}</div><div id=subMagnitude26>M{{subMagnitude[26]}}</div></div><div id=subMaxInt26 :style="{'background-color':subMaxIntColor[26]}"><span style="position:relative; top:-2px;">{{subMaxInt[26]}}</span></div></div>
        <div id=subBar27><div id=subLeft27><div id=subTime27>{{subTime[27]}}</div><div id=subEpicenter27 :style="{'font-size':subEpicenterFontSize[27]}">{{subEpicenter[27]}}</div><div id=subMagnitude27>M{{subMagnitude[27]}}</div></div><div id=subMaxInt27 :style="{'background-color':subMaxIntColor[27]}"><span style="position:relative; top:-2px;">{{subMaxInt[27]}}</span></div></div>
        <div id=subBar28><div id=subLeft28><div id=subTime28>{{subTime[28]}}</div><div id=subEpicenter28 :style="{'font-size':subEpicenterFontSize[28]}">{{subEpicenter[28]}}</div><div id=subMagnitude28>M{{subMagnitude[28]}}</div></div><div id=subMaxInt28 :style="{'background-color':subMaxIntColor[28]}"><span style="position:relative; top:-2px;">{{subMaxInt[28]}}</span></div></div>
        <div id=subBar29><div id=subLeft29><div id=subTime29>{{subTime[29]}}</div><div id=subEpicenter29 :style="{'font-size':subEpicenterFontSize[29]}">{{subEpicenter[29]}}</div><div id=subMagnitude29>M{{subMagnitude[29]}}</div></div><div id=subMaxInt29 :style="{'background-color':subMaxIntColor[29]}"><span style="position:relative; top:-2px;">{{subMaxInt[29]}}</span></div></div>
        <div id=subBar30><div id=subLeft30><div id=subTime30>{{subTime[30]}}</div><div id=subEpicenter30 :style="{'font-size':subEpicenterFontSize[30]}">{{subEpicenter[30]}}</div><div id=subMagnitude30>M{{subMagnitude[30]}}</div></div><div id=subMaxInt30 :style="{'background-color':subMaxIntColor[30]}"><span style="position:relative; top:-2px;">{{subMaxInt[30]}}</span></div></div>
        <div id=subBar31><div id=subLeft31><div id=subTime31>{{subTime[31]}}</div><div id=subEpicenter31 :style="{'font-size':subEpicenterFontSize[31]}">{{subEpicenter[31]}}</div><div id=subMagnitude31>M{{subMagnitude[31]}}</div></div><div id=subMaxInt31 :style="{'background-color':subMaxIntColor[31]}"><span style="position:relative; top:-2px;">{{subMaxInt[31]}}</span></div></div>
        <div id=subBar32><div id=subLeft32><div id=subTime32>{{subTime[32]}}</div><div id=subEpicenter32 :style="{'font-size':subEpicenterFontSize[32]}">{{subEpicenter[32]}}</div><div id=subMagnitude32>M{{subMagnitude[32]}}</div></div><div id=subMaxInt32 :style="{'background-color':subMaxIntColor[32]}"><span style="position:relative; top:-2px;">{{subMaxInt[32]}}</span></div></div>
        <div id=subBar33><div id=subLeft33><div id=subTime33>{{subTime[33]}}</div><div id=subEpicenter33 :style="{'font-size':subEpicenterFontSize[33]}">{{subEpicenter[33]}}</div><div id=subMagnitude33>M{{subMagnitude[33]}}</div></div><div id=subMaxInt33 :style="{'background-color':subMaxIntColor[33]}"><span style="position:relative; top:-2px;">{{subMaxInt[33]}}</span></div></div>
        <div id=subBar34><div id=subLeft34><div id=subTime34>{{subTime[34]}}</div><div id=subEpicenter34 :style="{'font-size':subEpicenterFontSize[34]}">{{subEpicenter[34]}}</div><div id=subMagnitude34>M{{subMagnitude[34]}}</div></div><div id=subMaxInt34 :style="{'background-color':subMaxIntColor[34]}"><span style="position:relative; top:-2px;">{{subMaxInt[34]}}</span></div></div>
        <div id=subBar35><div id=subLeft35><div id=subTime35>{{subTime[35]}}</div><div id=subEpicenter35 :style="{'font-size':subEpicenterFontSize[35]}">{{subEpicenter[35]}}</div><div id=subMagnitude35>M{{subMagnitude[35]}}</div></div><div id=subMaxInt35 :style="{'background-color':subMaxIntColor[35]}"><span style="position:relative; top:-2px;">{{subMaxInt[35]}}</span></div></div>
        <div id=subBar36><div id=subLeft36><div id=subTime36>{{subTime[36]}}</div><div id=subEpicenter36 :style="{'font-size':subEpicenterFontSize[36]}">{{subEpicenter[36]}}</div><div id=subMagnitude36>M{{subMagnitude[36]}}</div></div><div id=subMaxInt36 :style="{'background-color':subMaxIntColor[36]}"><span style="position:relative; top:-2px;">{{subMaxInt[36]}}</span></div></div>
        <div id=subBar37><div id=subLeft37><div id=subTime37>{{subTime[37]}}</div><div id=subEpicenter37 :style="{'font-size':subEpicenterFontSize[37]}">{{subEpicenter[37]}}</div><div id=subMagnitude37>M{{subMagnitude[37]}}</div></div><div id=subMaxInt37 :style="{'background-color':subMaxIntColor[37]}"><span style="position:relative; top:-2px;">{{subMaxInt[37]}}</span></div></div>
        <div id=subBar38><div id=subLeft38><div id=subTime38>{{subTime[38]}}</div><div id=subEpicenter38 :style="{'font-size':subEpicenterFontSize[38]}">{{subEpicenter[38]}}</div><div id=subMagnitude38>M{{subMagnitude[38]}}</div></div><div id=subMaxInt38 :style="{'background-color':subMaxIntColor[38]}"><span style="position:relative; top:-2px;">{{subMaxInt[38]}}</span></div></div>
        <div id=subBar39><div id=subLeft39><div id=subTime39>{{subTime[39]}}</div><div id=subEpicenter39 :style="{'font-size':subEpicenterFontSize[39]}">{{subEpicenter[39]}}</div><div id=subMagnitude39>M{{subMagnitude[39]}}</div></div><div id=subMaxInt39 :style="{'background-color':subMaxIntColor[39]}"><span style="position:relative; top:-2px;">{{subMaxInt[39]}}</span></div></div>
        <div id=subBar40><div id=subLeft40><div id=subTime40>{{subTime[40]}}</div><div id=subEpicenter40 :style="{'font-size':subEpicenterFontSize[40]}">{{subEpicenter[40]}}</div><div id=subMagnitude40>M{{subMagnitude[40]}}</div></div><div id=subMaxInt40 :style="{'background-color':subMaxIntColor[40]}"><span style="position:relative; top:-2px;">{{subMaxInt[40]}}</span></div></div>
        <div id=subBar41><div id=subLeft41><div id=subTime41>{{subTime[41]}}</div><div id=subEpicenter41 :style="{'font-size':subEpicenterFontSize[41]}">{{subEpicenter[41]}}</div><div id=subMagnitude41>M{{subMagnitude[41]}}</div></div><div id=subMaxInt41 :style="{'background-color':subMaxIntColor[41]}"><span style="position:relative; top:-2px;">{{subMaxInt[41]}}</span></div></div>
        <div id=subBar42><div id=subLeft42><div id=subTime42>{{subTime[42]}}</div><div id=subEpicenter42 :style="{'font-size':subEpicenterFontSize[42]}">{{subEpicenter[42]}}</div><div id=subMagnitude42>M{{subMagnitude[42]}}</div></div><div id=subMaxInt42 :style="{'background-color':subMaxIntColor[42]}"><span style="position:relative; top:-2px;">{{subMaxInt[42]}}</span></div></div>
        <div id=subBar43><div id=subLeft43><div id=subTime43>{{subTime[43]}}</div><div id=subEpicenter43 :style="{'font-size':subEpicenterFontSize[43]}">{{subEpicenter[43]}}</div><div id=subMagnitude43>M{{subMagnitude[43]}}</div></div><div id=subMaxInt43 :style="{'background-color':subMaxIntColor[43]}"><span style="position:relative; top:-2px;">{{subMaxInt[43]}}</span></div></div>
        <div id=subBar44><div id=subLeft44><div id=subTime44>{{subTime[44]}}</div><div id=subEpicenter44 :style="{'font-size':subEpicenterFontSize[44]}">{{subEpicenter[44]}}</div><div id=subMagnitude44>M{{subMagnitude[44]}}</div></div><div id=subMaxInt44 :style="{'background-color':subMaxIntColor[44]}"><span style="position:relative; top:-2px;">{{subMaxInt[44]}}</span></div></div>
        <div id=subBar45><div id=subLeft45><div id=subTime45>{{subTime[45]}}</div><div id=subEpicenter45 :style="{'font-size':subEpicenterFontSize[45]}">{{subEpicenter[45]}}</div><div id=subMagnitude45>M{{subMagnitude[45]}}</div></div><div id=subMaxInt45 :style="{'background-color':subMaxIntColor[45]}"><span style="position:relative; top:-2px;">{{subMaxInt[45]}}</span></div></div>
        <div id=subBar46><div id=subLeft46><div id=subTime46>{{subTime[46]}}</div><div id=subEpicenter46 :style="{'font-size':subEpicenterFontSize[46]}">{{subEpicenter[46]}}</div><div id=subMagnitude46>M{{subMagnitude[46]}}</div></div><div id=subMaxInt46 :style="{'background-color':subMaxIntColor[46]}"><span style="position:relative; top:-2px;">{{subMaxInt[46]}}</span></div></div>
        <div id=subBar47><div id=subLeft47><div id=subTime47>{{subTime[47]}}</div><div id=subEpicenter47 :style="{'font-size':subEpicenterFontSize[47]}">{{subEpicenter[47]}}</div><div id=subMagnitude47>M{{subMagnitude[47]}}</div></div><div id=subMaxInt47 :style="{'background-color':subMaxIntColor[47]}"><span style="position:relative; top:-2px;">{{subMaxInt[47]}}</span></div></div>
        <div id=subBar48><div id=subLeft48><div id=subTime48>{{subTime[48]}}</div><div id=subEpicenter48 :style="{'font-size':subEpicenterFontSize[48]}">{{subEpicenter[48]}}</div><div id=subMagnitude48>M{{subMagnitude[48]}}</div></div><div id=subMaxInt48 :style="{'background-color':subMaxIntColor[48]}"><span style="position:relative; top:-2px;">{{subMaxInt[48]}}</span></div></div>
        <div id=subBar49><div id=subLeft49><div id=subTime49>{{subTime[49]}}</div><div id=subEpicenter49 :style="{'font-size':subEpicenterFontSize[49]}">{{subEpicenter[49]}}</div><div id=subMagnitude49>M{{subMagnitude[49]}}</div></div><div id=subMaxInt49 :style="{'background-color':subMaxIntColor[49]}"><span style="position:relative; top:-2px;">{{subMaxInt[49]}}</span></div></div>
        <div id=subBar50><div id=subLeft50><div id=subTime50>{{subTime[50]}}</div><div id=subEpicenter50 :style="{'font-size':subEpicenterFontSize[50]}">{{subEpicenter[50]}}</div><div id=subMagnitude50>M{{subMagnitude[50]}}</div></div><div id=subMaxInt50 :style="{'background-color':subMaxIntColor[50]}"><span style="position:relative; top:-2px;">{{subMaxInt[50]}}</span></div></div>
    </div>
</template>

<script>
    //定义烈度配色
    const intColor = {
        "0":{
            "bkcolor":"#444444"
        },
        "1":{
            "bkcolor":"#9bc4e4"
        },
        "2":{
            "bkcolor":"#00a0f1"
        },
        "3":{
            "bkcolor":"#0062f5"
        },
        "4":{
            "bkcolor":"#2de161"
        },
        "5":{
            "bkcolor":"#1cac5d"
        },
        "6":{
            "bkcolor":"#ffbd2b"
        },
        "7":{
            "bkcolor":"#ff992b"
        },
        "8":{
            "bkcolor":"#fa5151"
        },
        "9":{
            "bkcolor":"#f4440d"
        },
        "10":{
            "bkcolor":"#ff000d"
        },
        "11":{
            "bkcolor":"#c20007"
        },
        "12":{
            "bkcolor":"#fd2fc2"
        }
    };
    import axios from 'axios';
    export default {
        name: 'ChineseEarthquakeList',
        data(){
            return{
                mainType: null,
                mainEpicenter: '载入中',
                mainMagnitude: '0.0',
                mainDepth: null,
                mainTime: '01/01 00:00',
                mainMaxInt: '-',
                mainMaxIntColor: '#444',

                subTime: ['01/01 00:00','01/01 00:00','01/01 00:00'],
                subEpicenter: ['载入中','载入中','载入中'],
                subMagnitude: ['0.0','0.0','0.0'],
                subMaxInt: ['-','-','-'],
                subMaxIntColor: ['#444','#444','#444'],
                subEpicenterFontSize: ['20px', '20px', '20px']
            }
        },
        methods:{
            init(){
                let subTime = [];
                let subEpicenter = [];
                let subMagnitude = [];
                let subMaxInt = [];
                let subMaxIntColor = [];

                for (let i=0; i<=50; i++){
                    subTime.push('01/01 00:00');
                    subEpicenter.push('载入中');
                    subMagnitude.push('0.0');
                    subMaxInt.push('-');
                    subMaxIntColor.push('#444');
                }
                this.subTime = subTime;
                this.subEpicenter = subEpicenter;
                this.subMagnitude = subMagnitude;
                this.subMaxInt = subMaxInt;
                this.subMaxIntColor = subMaxIntColor;

            },
            async getMainData(){
                axios.get('https://api.projectbs.cn/v2/ceic/get_data.json?' + new Date().getTime()).then(data => {
                    let json = data.data;
                    this.mainType = json.data.type;
                    this.mainDepth = json.data.depth;
                    this.mainEpicenter = json.data.epicenter;
                    let mainStartAt = json.data.occurTime;
                    this.mainMagnitude = json.data.magnitude;
                    //startAt 转换
                    mainStartAt = mainStartAt.replace("月", "/");
                    mainStartAt = mainStartAt.replace("日", " ");
                    mainStartAt = mainStartAt.replace("时", ":");
                    this.mainTime = mainStartAt.replace("分", "");

                    if (this.mainType == '正式') {
                        this.mainTime += ' 正式报';
                        this.mainMaxInt = this.calcMaxInt(this.mainMagnitude, this.mainDepth);
                        this.mainMaxIntColor = intColor[this.mainMaxInt].bkcolor;
                    }else if (this.mainType == '自动'){
                        this.mainDepth = '?';
                        this.mainTime += ' 自动报';
                        this.mainMaxInt = '-';
                        this.mainMaxIntColor = '#444';
                    }
                });
            },
            async getSubData(){
                axios.get('https://api.wolfx.jp/cenc_eqlist.json?' + new Date().getTime()).then(data => {
                    let json = data.data;
                    let subTime = [];
                    let subEpicenter = [];
                    let subMagnitude = [];
                    let subDepth = [];
                    let subMaxInt = [];
                    let subMaxIntColor = [];
                    for (let i=2; i<=50; i++){
                        subTime[i] = eval("json.No" + i + ".time");
                        subTime[i] = subTime[i].substring(5, 16);
                        subTime[i] = subTime[i].replace(/-/g, '/');
                        subEpicenter[i] = eval("json.No" + i + ".location");
                        subMagnitude[i] = eval("json.No" + i + ".magnitude");
                        subDepth[i] = eval("json.No" + i + ".depth");
                        subMaxInt[i] = this.calcMaxInt(subMagnitude[i], subDepth[i]);
                        subMaxIntColor[i] = intColor[subMaxInt[i]].bkcolor;
                        if (subEpicenter[i].indexOf('（有感）') != -1 || subEpicenter[i].indexOf('(有感)') != -1){
                            subEpicenter[i] = subEpicenter[i].replace('（有感）', '');
                            subEpicenter[i] = subEpicenter[i].replace('(有感)', '');
                            subTime[i] += ' 有感';
                        }
                        if (subDepth[i] >= 150) subTime[i] += ' 深源';
                        this.calcSubEpicenterFontSize(subEpicenter[i], i);
                    }
                    this.subTime = subTime;
                    this.subEpicenter = subEpicenter;
                    this.subMagnitude = subMagnitude;
                    this.subMaxInt = subMaxInt;
                    this.subMaxIntColor = subMaxIntColor;
                })
            },
            calcMaxInt(calcMagnitude, calcDepth){
                let numa = 1.65*calcMagnitude;
                let numb = calcDepth<10 ? 1.21*Math.log10(10) : 1.21*Math.log10(calcDepth);
                let maxInt = Math.round(numa/numb);
                return (maxInt);
            },
            calcSubEpicenterFontSize(epicenter, i){
                if (epicenter.length >= 12){
                    this.subEpicenterFontSize[i] = '18px';
                }else{
                    this.subEpicenterFontSize[i] = '20px';
                }
            }
        },
        created:function(){
            this.init();
            this.getMainData();
            this.getSubData();
            setInterval(() => {
                this.getMainData();
                this.getSubData();
            }, 5000);
        }
    }
</script>

<style>
    @font-face {
        font-family:'oppoSans-H';
        src:url('../assets/font/OPPOSans-H.ttf') format('truetype');
    }
    @font-face {
        font-family:'oppoSans-B';
        src:url('../assets/font/OPPOSans-B.ttf') format('truetype');
    }
    * {
        font-family:oppoSans-B,sans-serif;
        padding:0;
        margin:0;
        font-variant-numeric: tabular-nums;
    }
    body {
        font-family:oppoSans-B,sans-serif;
        margin:0 auto;
        background-color:#242424;
    }
    #mainBar {
	position:relative;
	top:0px;
	left:0px;
	height:98px;
	width:350px;
	color:white;
    }
    #mainLeft {
        position:absolute;
        top:0px;
        left:0px;
        height:98px;
        width:248px;
        background-color:#333333;
        border-radius:10px;
    }
    #mainMaxInt {
        position:absolute;
        height:98px;
        width:98px;
        right:0px;
        background-color:#444444;
        border-radius:10px;
        line-height:98px;
        font-size:64px;
        font-family:OPPOSans-H;
        text-align:center;
        text-shadow:0px 4px 10px rgba(0,0,0,0.3);
        border: 3px solid white;
        box-sizing:border-box;
    }
    #mainTime {
        position:relative;
        top:2px;
        left:4px;
        font-size:16px;
    }
    #mainEpicenter {
        position:relative;
        top:2px;
        left:4px;
        font-size:20px;
        line-height:22px;
        width:237px;
    }
    #mainDepth {
        position:absolute;
        bottom:0px;
        left:4px;
        font-size:25px;
    }
    #mainMagnitude {
        position:absolute;
        bottom:0px;
        right:4px;
        font-size:25px;
    }
    [id^="subBar"] {
        position:relative;
        left:0px;
        height:48px;
        width:350px;
        color:white;
        margin-top:4px;
    }
    [id^="subLeft"] {
        position:absolute;
        top:0px;
        left:0px;
        height:48px;
        width:298px;
        background-color:#333333;
        border-radius:10px;
    }
    [id^="subMaxInt"] {
        position:absolute;
        right:0px;
        top:0px;
        height:48px;
        width:48px;
        background-color:#444444;
        border-radius:10px;
        line-height:48px;
        font-size:30px;
        font-family:OPPOSans-H;
        text-align:center;
        text-shadow:0px 4px 10px rgba(0,0,0,0.3);
        border: 2px solid white;
        box-sizing:border-box;
    }
    [id^="subTime"] {
        position:relative;
        top:2px;
        left:4px;
        font-size:15px;
    }
    [id^="subEpicenter"] {
        position:relative;
        top:2px;
        left:4px;
        font-size:20px;
    }
    [id^="subMagnitude"] {
        position:absolute;
        right:4px;
        font-size:21px;
        line-height:48px;
        top:0px;
    }
</style>