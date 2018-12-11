#include <iostream>
#include <iomanip>
using namespace std;

int main () {

    //Finals
    int R1game1F;
    int R1game2F;
    string FR1game1F;
    string FR1game2F;

    //Third place
    int R1game1T;
    int R1game2T;
    string FR1game1T;
    string FR1game2T;

    //Qualified teams
    
    //Qulified in 1st place from group A
    int Q1groupA;
    string FQ1groupA;


    //Qulified in 1st place from group B
    int Q1groupB;
    string FQ1groupB;

    //Qualified in 2nd place from group A
    int Q2groupA;
    string FQ2groupA;

    //Qualified in 2nd place from group B
    int Q2groupB;
    string FQ2groupB;
    
    //Qualified teams' attack, midfield, deffence of round 1
    int Q1groupAattack, Q1groupBattack, Q2groupAattack, Q2groupBattack;
    int Q1groupAmidfield, Q1groupBmidfield, Q2groupAmidfield, Q2groupBmidfield;
    int Q1groupAdeffence, Q1groupBdeffence, Q2groupAdeffence, Q2groupBdeffence;
    
    //Finals teams' attack, midfield, deffence of round 1
    int R1game1Fattack, R1game2Fattack;
    int R1game1Fmidfield, R1game2Fmidfield;
    int R1game1Fdeffence, R1game2Fdeffence;

    //Match for third place teams' attack, midfield, deffence of round 1
    int R1game1Tattack, R1game2Tattack;
    int R1game1Tmidfield, R1game2Tmidfield;
    int R1game1Tdeffence, R1game2Tdeffence;

    //group A (Italy, Portugal, Australia, Iran)

    int portugal = 0, italy = 0, australia = 0, iran = 0;
    
    int italyattack = 90;
    int portugalattack = 82;
    int australiaattack = 85;
    int iranattack = 81;

    int italymidfield = 92;
    int portugalmidfield = 83;
    int australiamidfield = 81;
    int iranmidfield = 83;

    int italydeffence = 85;
    int portugaldeffence = 81;
    int australiadeffence = 79;
    int irandeffence = 75;

    //group B (Croatia, Belgium, Denmark, Columbia)

    int croatia = 0, belgium = 0, denmark = 0, columbia = 0;

    int croatiaattack = 87;
    int belgiumattack = 89;
    int denmarkattack = 83;
    int columbiaattack = 85;

    int croatiamidfield = 90;
    int belgiummidfield = 89;
    int denmarkmidfield = 83;
    int columbiamidfield = 86;

    int croatiadeffence = 87;
    int belgiumdeffence = 88;
    int denmarkdeffence = 84;
    int columbiadeffence = 82;
    
    
    //group C (Chile, Sweden, Netherlands, Mexico)
    
    int chile = 0, sweden = 0, netherlands = 0, mexico = 0;
    
    int chileattack = 85;
    int swedenattack = 84;
    int netherlandsattack = 92;
    int mexicoattack = 87;
    
    int chilemidfield = 80;
    int swedenmidfield = 85;
    int netherlandsmidfield = 86;
    int mexicomidfield = 84;
    
    int chiledeffence = 75;
    int swedendeffence = 80;
    int netherlandsdeffence = 85;
    int mexicodeffence = 80;
    
    //group D (Wales, Poland, USA, Peru)

    int wales = 0, poland = 0, usa = 0, peru = 0;

    int walesattack = 70;
    int polandattack = 70;
    int usaattack = 65;
    int peruattack = 75;

    int walesmidfield = 70;
    int polandmidfield = 75;
    int usamidfield = 68;
    int perumidfield = 75;

    int walesdeffence = 72;
    int polanddeffence = 79;
    int usadeffence = 80;
    int perudeffence = 78;
     
     //group E (Brazil, Germany, Senegal, Austria)

     int brazil = 0, germany = 0, senegal = 0, austria = 0;

     int brazilattack = 90;
     int germanyattack = 95;
     int senegalattack = 70;
     int austriaattack = 75;

     int brazilmidfield = 95;
     int germanymidfield = 90;
     int senegalmidfield = 88;
     int austriamidfield = 80;

     int brazildeffence = 90;
     int germanydeffence = 95;
     int senegaldeffence = 90;
     int austriadeffence = 75;

     //group F (Romania, Iceland, England, Spain)

     int romania = 0, iceland = 0, england = 0, spain = 0;

     int romaniaattack = 78;
     int icelandattack = 75;
     int englandattack = 90;
     int spainattack = 90;

     int romaniamidfield = 75;
     int icelandmidfield = 80;
     int englandmidfield = 93;
     int spainmidfield = 95;

     int romaniadeffence = 80;
     int icelanddeffence = 79;
     int englanddeffence = 90;
     int spaindeffence = 95;

     //group G (Argentina, France, Turkey, Russia) 

     int argentina = 0, france = 0, turkey = 0, russia = 0

     int argentinaattack = 95;
     int franceattack = 95;
     int turkeyattack = 70;
     int russiaattack = 70;

     int argentinamidfield = 90;
     int francemidfield = 95;
     int turkeymidfield = 92;
     int russiamidfield = 80;

     int argentinadeffence = 90;
     int francedeffence = 90;
     int turkeydeffence = 80;
     int russiadeffence = 70;

     //group H (Uruguay, Serbia, Venezuela, Morocco)

     int uruguay = 0, serbia = 0, venezuela = 0, morocco = 0;

     int uruguayattack = 90;
     int serbiaattack = 60;
     int venezuelaattack = 80;
     int moroccoattack = 70;

     int uruguaymidfield = 85;
     int serbiamidfield = 90;
     int venezuelamidfield = 70;
     int moroccomidfield = 70;

     int uruguaydeffence = 80;
     int serbiadeffence = 80;
     int venezueladeffence = 80;
     int moroccodeffence = 75;

     //group H

     //attack of uruguay
     if (uruguayattack > serbiaattack) {
         uruguay += 1;
     }
     if (uruguayattack > venezuelaattack) {
         uruguay += 1;
     }
     if (uruguayattack > moroccoattack) {
         uruguay += 1;
     }

     //attack of serbia
     if (serbiaattack > uruguayattack) {
         serbia += 1;
     }
     if (serbiaattack > venezuelaattack) {
         serbia += 1;
     }
     if (serbiaattack > moroccoattack) {
         serbia += 1;
     }

     //attack of venezuela
     if (venezuelaattack > uruguayattack) {
         venezuela += 1;
     } 
     if (venezuelaattack > serbiaattack) {
         venezuela += 1;
     }
     if (venezuelaattack > moroccoattack) {
         venezuela += 1;
     }

     //attack of morocco
     if (moroccoattack > uruguayattack) {
         morocco += 1;
     }
     if (moroccoattack > serbiaattack) {
         morocco += 1;
     }
     if (moroccoattack > venezuelaattack) {
         morocco += 1;
     }

     //midfield of uruguay
     if (uruguaymidfield > serbiamidfield) {
         uruguay += 1;
     }
     if (uruguaymidfield > venezuelamidfield) {
         uruguay += 1;
     }
     if (uruguaymidfield > moroccomidfield) {
         uruguay += 1;
     }

     //midfield of serbia
     if (serbiamidfield > uruguaymidfield ) {
         serbia += 1;
     }
     if (serbiamidfield > venezuelamidfield ) {
         serbia += 1;
     }
     if (serbiamidfield > moroccomidfield ) {
         serbia += 1;
     }

     //midfield of venezuela
     if (venezuelamidfield > uruguaymidfield) {
         venezuela += 1;
     }
     if (venezuelamidfield > serbiamidfield) {
         venezuela += 1;
     }
     if (venezuelamidfield > morocoomidfield) {
         venezuela += 1;
     }

     //midfield of morocco
     if (moroccomidfield > uruguaymidfield) {
         morocoo += 1;
     }
     if (moroccomidfield > serbiamidfield) {
         morocoo += 1;
     }
     if (moroccomidfield > venezuelamidfield) {
         morocoo += 1;
     }

     //defense of uruguay
     if (uruguaydeffence > serbiadeffence) {
         uruguay += 1;
     }
     if (uruguaydeffence > venezueladeffence) {
         uruguay += 1;
     }
     if (uruguaydeffence > moroccodeffence) {
         uruguay += 1;
     }

     //defense of venezuela
     if (venezueladeffence > serbiadeffence) {
         venezuela += 1;
     }
     if (venezueladeffence > uruguaydeffence) {
         venezuela += 1;
     }
     if (venezueladeffence > moroccodeffence) {
         venezuela += 1;
     }

     //defense of serbia
     if (serbiadeffence > uruguaydeffence) {
         serbia += 1;
     }
     if (serbiadeffence > venezueladeffence) {
         serbia += 1;
     }
     if (serbiadeffence > moroccodeffence) {
         serbia += 1;
     }

     //defense of morocco
     if (moroccodeffence > uruguaydeffence) {
         morocoo += 1;
     }
     if (moroccodeffence > serbiadeffence) {
         morocoo += 1;
     }
     if (moroccodeffence > venezueladeffence) {
         morocoo += 1;
     }

     //1st place result of group H
    if (uruguay > serbia && uruguay > morocco && uruguay > vennezuela) {
        cout << "Uruguay is the winner of Group H" << endl;
        Q1groupH = uruguay;
        Q1groupHattack = uruguayattack;
        Q1groupHmidfield = uruguaymidfield;
        Q1groupHdeffence = uruguaydeffence;
        FQ1groupH = "Uruguay";
    }
    else if (serbia > uruguay && serbia > morocco && serbia > venezuela) {
        cout << "Serbia is the winner of Group H" << endl;
        Q1groupH = serbia;
        Q1groupHattack = serbiaattack;
        Q1groupHmidfield = serbiamidfield;
        Q1groupHdeffence = serbiadeffence;
        FQ1groupH = "Serbia";
    }
    else if (morocoo > uruguay && morocco > serbia && morocco > venezuela) {
        cout << "Morocco is the winner of Group H" << endl;
        Q1groupH = morocco;
        Q1groupHattack = moroccoattack;
        Q1groupHmidfield = moroccomidfield;
        Q1groupHdeffence = moroccodeffence;
        FQ1groupH = "Morocco";
    }
    else if (venezuela > uruguay && venezuela > morocco && venezuela > serbia) {
        cout << "Venezuela is the winner of Group H" << endl;
        Q1groupH = venezuela;
        Q1groupHattack = venezuelaattack;
        Q1groupHmidfield = venezuelamidfield;
        Q1groupHdeffence = venezueladeffence;
        FQ1groupH = "Venezuela";

        //2nd place results of group H 


        //uruguay
        if (uruguay > serbia && uruguay > morocco && uruguay < venezuela) {
        cout << "Uruguay is the second of Group H" << endl;
        Q2groupH = uruguay;
        Q2groupHattack = uruguayattack;
        Q2groupHmidfield = uruguaymidfield;
        Q2groupHdeffence = uruguaydeffence;
        FQ2groupH = "Uruguay";
        FR1game1F = "Uruguay";
        FR1game1T = "Uruguay";
    }

    else if (uruguay > serbia && uruguay < morocco && uruguay > venezuela) {
        cout << "Uruguay is the second of Group H" << endl;
        Q2groupH = uruguay;
        Q2groupHattack = uruguayattack;
        Q2groupHmidfield = uruguaymidfield;
        Q2groupHdeffence = uruguaydeffence;
        FQ2groupH = "Uruguay";
        FR1game1F = "Uruguay";
        FR1game1T = "Uruguay";
    }

    else if (uruguay < serbia && uruguay < morocco && uruguay > venezuela) {
        cout << "Uruguay is the second of Group H" << endl;
        Q2groupH = uruguay;
        Q2groupHattack = uruguayattack;
        Q2groupHmidfield = uruguaymidfield;
        Q2groupHdeffence = uruguaydeffence;
        FQ2groupH = "Uruguay";
        FR1game1F = "Uruguay";
        FR1game1T = "Uruguay";
    }

    else {}


    //serbia
    if (serbia > uruguay && serbia > morocco && serbia < venezuela) {
        cout << "Serbia is the second of Group H" << endl;
        Q2groupH = serbia;
        Q2groupHattack = serbiaattack;
        Q2groupHmidfield = serbiamidfield;
        Q2groupHdeffence = serbiadeffence;
        FQ2groupH = "Serbia";
        FR1game1F = "Serbia";
        FR1game1T = "Serbia";
    }
    else if (serbia > uruguay && serbia < morocco && serbia > venezuela) {
        cout << "Serbia is the second of Group H" << endl;
        Q2groupH = serbia;
        Q2groupHattack = serbiaattack;
        Q2groupHmidfield = serbiamidfield;
        Q2groupHdeffence = serbiadeffence;
        FQ2groupH = "Serbia";
        FR1game1F = "Serbia";
        FR1game1T = "Serbia";
    }
    else if (serbia < uruguay && serbia < morocco && serbia > venezuela) {
        cout << "Serbia is the second of Group H" << endl;
        Q2groupH = serbia;
        Q2groupHattack = serbiaattack;
        Q2groupHmidfield = serbiamidfield;
        Q2groupHdeffence = serbiadeffence;
        FQ2groupH = "Serbia";
        FR1game1F = "Serbia";
        FR1game1T = "Serbia";
    }
    else {}

    //venezuela
    if (venezuela > uruguay && venezuela > morocco && venezuela < serbia) {
        cout << "Venezuela is the second of Group H" << endl;
        Q2groupH = venezuela;
        Q2groupHattack = venezuelaattack;
        Q2groupHmidfield = venezuelamidfield;
        Q2groupHdeffence = venezueladeffence;
        FQ2groupH = "Venezuela";
        FR1game1F = "Venezuela";
        FR1game1T = "Venezuela";
    }
    else if (venezuela > uruguay && venezuela < morocco && venezuela > serbia) {
        cout << "Venezuela is the second of Group H" << endl;
        Q2groupH = venezuela;
        Q2groupHattack = venezuelaattack;
        Q2groupHmidfield = venezuelamidfield;
        Q2groupHdeffence = venezueladeffence;
        FQ2groupH = "Venezuela";
        FR1game1F = "Venezuela";
        FR1game1T = "Venezuela";
    }
    else if (venezuela < uruguay && venezuela < morocco && venezuela > serbia) {
        cout << "Venezuela is the second of Group H" << endl;
        Q2groupH = venezuela;
        Q2groupHattack = venezuelaattack;
        Q2groupHmidfield = venezuelamidfield;
        Q2groupHdeffence = venezueladeffence;
        FQ2groupH = "Venezuela";
        FR1game1F = "Venezuela";
        FR1game1T = "Venezuela";
    }
    else {}

    //morocco
    if (morocco > uruguay && morocco > venezuela && morocco < serbia) {
        cout << "Morocco is the second of Group H" << endl;
        Q2groupH = venezuela;
        Q2groupHattack = venezuelaattack;
        Q2groupHmidfield = venezuelamidfield;
        Q2groupHdeffence = venezueladeffence;
        FQ2groupH = "Venezuela";
        FR1game1F = "Venezuela";
        FR1game1T = "Venezuela";
    }
    else if (venezuela > uruguay && venezuela < morocco && venezuela > serbia) {
        cout << "Venezuela is the second of Group H" << endl;
        Q2groupH = venezuela;
        Q2groupHattack = venezuelaattack;
        Q2groupHmidfield = venezuelamidfield;
        Q2groupHdeffence = venezueladeffence;
        FQ2groupH = "Venezuela";
        FR1game1F = "Venezuela";
        FR1game1T = "Venezuela";
    }
    else if (venezuela < uruguay && venezuela < morocco && venezuela > serbia) {
        cout << "Venezuela is the second of Group H" << endl;
        Q2groupH = venezuela;
        Q2groupHattack = venezuelaattack;
        Q2groupHmidfield = venezuelamidfield;
        Q2groupHdeffence = venezueladeffence;
        FQ2groupH = "Venezuela";
        FR1game1F = "Venezuela";
        FR1game1T = "Venezuela";
    }
    else {}



    }
     //group G

     //attack of argentina
     if (argentinaattack > franceattack) {
         argentina += 1;
     }
     if (argentinaattack > turkeyattack) {
         argentina += 1;
     }
     if (argentinaattack > russiaattack) {
         argentina += 1;
     }

     //attack of france
     if (franceattack > argentinaattack) { 
         franceattack += 1;
     }
     if (franceattack > turkeyattack) { 
         franceattack += 1;
     }
     if (franceattack > russiaattack) { 
         franceattack += 1;
     }

     //attack of turkey
     if (turkeyattack > argentinaattack) {
         turkey += 1;
     }
     if (turkeyattack > franceattack) {
         turkey += 1;
     }
     if (turkeyattack > russiaattack) {
         turkey += 1;
     }

     //attack of russia
     if (russiaattack > argentinaattack) {
         russia += 1;
     }
     if (russiaattack > franceattack) {
         russia += 1;
     }
     if (russiaattack > turkeyattack) {
         russia += 1;
     }

     //midfield of argentina 
    if (argentinamidfield > francemidfield) {
         argentina += 1;
     }
     if (argentinamidfield > turkeymidfield) {
         argentina += 1;
     }
     if (argentinamidfield > russiamidfield) {
         argentina += 1;
     }

     //midfield of france
     if (francemidfield > argentinamidfield) {
         france += 1;
     }
     if (francemidfield > turkeymidfield) {
         france += 1;
     }
     if (francemidfield > russiamidfield) {
         france += 1;
     }

     //midfield of turkey
     if (turkeymidfield > argentinamidfield) {
         turkey += 1;
     }
     if (turkeymidfield > francemidfield) {
         turkey += 1;
     }
     if (turkeymidfield > russiamidfield) {
         turkey += 1;
     }

     //midfield of russia
     if (russiamidfield > argentinamidfield) {
         russia += 1;
     }
     if (russiamidfield > francemidfield) {
         russia += 1;
     }
     if (russiamidfield > turkeymidfield) {
         russia += 1;
     }

     //defense of argentina
     if (argentinadeffence > francedeffence) {
         argentina += 1;
     }
     if (argentinadeffence > turkeydeffence) {
         argentina += 1;
     }
     if (argentinadeffence > russiadeffence) {
         argentina += 1;
     }

     //defense of france
     if (francedeffence > argentinadeffence) {
         france += 1;
     }
     if (francedeffence > turkeydeffence) {
         france += 1;
     }
     if (francedeffence > russiadeffence) {
         france += 1;
     }

     //defense of turkey
     if (turkeydeffence > argentinadeffence) {
         turkey += 1;
     }
     if (turkeydeffence > francedeffence) {
         turkey += 1;
     }
     if (turkeydeffence > russiadeffence) {
         turkey += 1;
     }

     //defense of russia
     if (russiadeffence > argentinadeffence) {
         russia += 1;
     }
     if (russiadeffence > francedeffence) {
         russia += 1;
     }
     if (russiadeffence > turkeydeffence) {
         russia += 1;
     }

     //1st place results of group G
     if (argentina > russia && argentina > france && argentina > turkey) {
        cout << "Argentina is the winner of Group G" << endl;
        Q1groupG = argentina;
        Q1groupGattack = argentinaattack;
        Q1groupGmidfield = argentinamidfield;
        Q1groupGdeffence = argentinadeffence;
        FQ1groupG = "Argentina";
    }
    else if (russia > argentina && russia > france && russia > turkey) {
        cout << "Russia is the winner of Group G" << endl;
        Q1groupG = russia;
        Q1groupGattack = russiaattack;
        Q1groupGmidfield = russiamidfield;
        Q1groupGdeffence = russiadeffence;
        FQ1groupG = "Russia";
    }
    else if (france > argentina && france > russia && france > turkey) {
        cout << "France is the winner of Group G" << endl;
        Q1groupG = france;
        Q1groupGattack = franceattack;
        Q1groupGmidfield = francemidfield;
        Q1groupGdeffence = francedeffence;
        FQ1groupG = "France";
    }
    else if (turkey > argentina && turkey > france && turkey > russia) {
        cout << "Turkey is the winner of Group G" << endl;
        Q1groupG = turkey;
        Q1groupGattack = turkeyattack;
        Q1groupGmidfield = turkeymidfield;
        Q1groupGdeffence = turkeydeffence;
        FQ1groupG = "Turkey";
    }


     //group F

     //attack of romania
     if (romaniaattack > icelandattack) {
         romania += 1;
     }
     if (romaniaattack > englandattack) {
         romania += 1;
     }
     if (romaniaattack > spainattack) {
         romania += 1;
     }

     //attack of iceland
     if (icelandattack > romaniaattack) [
         iceland += 1;
     ]
     if (icelandattack > englandattack) [
         iceland += 1;
     ]
     if (icelandattack > spainattack) [
         iceland += 1;
     ]

     //attack of england
     if (englandattack > romaniaattack) {
         england += 1;
     }
     if (englandattack > icelandattack) {
         england += 1;
     }
     if (englandattack > spainattack) {
         england += 1;
     }

     //attack of spain
     if (spainattack > romaniaattack) {
         spain += 1;
     }
     if (spainattack > englandattack) {
         spain += 1;
     }
     if (spainattack > icelandattack) {
         spain += 1;
     }

     //midfield of romania
     if (romaniamidfield > englandmidfield) {
         romania += 1;
     }
     if (romaniamidfield > icelandmidfield) {
         romania += 1;
     }
     if (romaniamidfield > spainmidfield) {
         romania += 1;
     }
     
     //midfield of england
     if (englandmidfield > romaniamidfield) {
         england += 1;
     }
     if (englandmidfield > icelandmidfield) {
         england += 1;
     }
     if (englandmidfield > spainmidfield) {
         england += 1;
     }

     //midfield of iceland
     if (icelandmidfield > romaniamidfield) {
         iceland += 1;
     }
     if (icelandmidfield > englandmidfield) {
         iceland += 1;
     }
     if (icelandmidfield > spainmidfield) {
         iceland += 1;
     }

     //midfield of spain
     if (spainmidfield > romaniamidfield) {
         spain += 1;
     }
     if (spainmidfield > englandmidfield) {
         spain += 1;
     }
     if (spainmidfield > icelandmidfield) {
         spain += 1;
     } 

     //defense of romania
     if (romaniadeffence > englanddeffence) {
         romania += 1;
     }
     if (romaniadeffence > icelanddeffence) {
         romania += 1;
     }
     if (romaniadeffence > spaindeffence) {
         romania += 1;
     }

     //defense of england
     if (englanddeffence > romaniadeffence) {
         england += 1;
     }
     if (englanddeffence > icelanddeffence) {
         england += 1;
     }
     if (englanddeffence > spaindeffence) {
         england += 1;
     }

     //defense of iceland
     if (icelanddeffence > romaniadeffence) {
         iceland += 1;
     }
     if (icelanddeffence > englanddeffence) {
         iceland += 1;
     }
     if (icelanddeffence > spaindeffence) {
         iceland += 1;
     }

     //defense of spain
     if (spaindeffence > romaniadeffence) {
         spain += 1;
     }
     if (spaindeffence > englanddeffence) {
         spain += 1;
     }
     if (spaindeffence > icelanddeffence) {
         spain += 1;
     } 

     //1st place results of group F
     if (spain > romania && spain > england && spain > iceland) {
        cout << "Spain is the winner of Group F" << endl;
        Q1groupF = spain;
        Q1groupFattack = spainattack;
        Q1groupFmidfield = spainmidfield;
        Q1groupFdeffence = spaindeffence;
        FQ1groupF = "Spain";
    }
    else if (romania > spain && romania > england && romania > iceland) {
        cout << "Romania is the winner of Group F" << endl;
        Q1groupF = romania;
        Q1groupFattack = romaniaattack;
        Q1groupFmidfield = romaniamidfield;
        Q1groupFdeffence = romaniadeffence;
        FQ1groupF = "Romania";
    }
    else if (england > spain && england > romania&& england > iceland) {
        cout << "England is the winner of Group F" << endl;
        Q1groupF = england;
        Q1groupFattack = englandattack;
        Q1groupFmidfield = englandmidfield;
        Q1groupFdeffence = englanddeffence;
        FQ1groupF = "England";
    }
    else if (iceland > spain && iceland > england && iceland > romania) {
        cout << "Iceland is the winner of Group F" << endl;
        Q1groupF = iceland;
        Q1groupFattack = icelandattack;
        Q1groupFmidfield = icelandmidfield;
        Q1groupFdeffence = icelanddeffence;
        FQ1groupF = "Iceland";
    }

     //group E 
      
    //attack of brazil
    if (brazilattack > germanyattack) {
        brazil += 1;
    }
    if (brazilattack > senegalattack) {
        brazil += 1;
    }
    if (brazilattack > austriaattack) {
        brazil += 1;
    }

    //attack of germany
    if (germanyattack > brazilattack) {
        germany += 1;
    } 
    if (germanyattack > senegalattack) {
        germany += 1;
    } 
    if (germanyattack > austriaattack) {
        germany += 1;
    } 

    //attack of senegal
    if (senegalattack > brazilattack) {
        senegal += 1;
    }
    if (senegalattack > germanyattack) {
        senegal += 1;
    }
    if (senegalattack > austriaattack) {
        senegal += 1;
    }

    //attack of austria
    if (austriaattack > brazilattack) {
        austria += 1;
    } 
    if (austriaattack > germanyattack) {
        austria += 1;
    }
    if (austriaattack > senegalattack) {
        austria += 1;
    } 

    //midfield of brazil 
    if (brazilmidfield > germanymidfield) {
        brazil += 1;
    }
    if (brazilmidfield > senegalmidfield) {
        brazil += 1;
    }
    if (brazilmidfield > austriamidfield) {
        brazil += 1;
    }

    //midfield of germany
    if (germanymidfield > brazilmidfield) {
        germany += 1;
    }
    if (germanymidfield > senegalmidfield) {
        germany += 1;
    }
    if (germanymidfield > austriamidfield) {
        germany += 1;
    }

    //midfield of senegal
    if (senegalmidfield > brazilmidfield) {
        senegal += 1;
    }
    if (senegalmidfield > germanymidfield) {
        senegal += 1;
    }
    if (senegalmidfield > austriamidfield) {
        senegal += 1;
    }

    //midfield of austria
    if (austriamidfield > brazilmidfield) {
        austria += 1;
    }
    if (austriamidfield > germanymidfield) {
        austria += 1;
    }
    if (austriamidfield > senegalmidfield) {
        austria += 1;
    }

    //defense of brazil
    if (brazildeffence > germanydeffence) {
        brazil += 1;
    }
    if (brazildeffence > senegaldeffence) {
        brazil += 1;
    }
    if (brazildeffence > austriadeffence) {
        brazil += 1;
    }

    //defense of germany
    if (germanydeffence > brazildeffence) {
        germany += 1;
    }
    if (germanydeffence > senegaldeffence) {
        germany += 1;
    }
    if (germanydeffence > austriadeffence) {
        germany += 1;
    }

    //defense of senegal 
    if (senegaldeffence > brazildeffence) {
        senegal += 1;
    }
    if (senegaldeffence > germanydeffence) {
        senegal += 1;
    }
    if (senegaldeffence > austriadeffence) {
        senegal += 1;
    }

    //defense of austria
    if (austriadeffence > brazildeffence) {
        austria += 1;
    }
    if (austriadeffence > germanydeffence) {
        austria += 1;
    }
    if (austriadeffence > senegaldeffence) {
        austria += 1;
    }

    //1st place results of group E
   if (brazil > germany && brazil > austria && brazil > senegal) {
        cout << "Brazil is the winner of Group E" << endl;
        Q1groupE = brazil;
        Q1groupEattack = brazilattack;
        Q1groupEmidfield = brazilmidfield;
        Q1groupEdeffence = brazildeffence;
        FQ1groupE = "Brazil";
    }
    else if (germany > brazil && germany > austria && germany > senegal) {
        cout << "Germany is the winner of Group E" << endl;
        Q1groupE = germany;
        Q1groupEattack = germanyattack;
        Q1groupEmidfield = germanymidfield;
        Q1groupEdeffence = germanydeffence;
        FQ1groupE = "Germany";
    }
    else if (austria > germany && austria > germany && austria > senegal) {
        cout << "Austria is the winner of Group E" << endl;
        Q1groupE = austria;
        Q1groupEattack = austriaattack;
        Q1groupEmidfield = austriamidfield;
        Q1groupEdeffence = austriadeffence;
        FQ1groupE = "Austria";
    }
    else if (senegal > germany && senegal > germany && senegal > austria) {
        cout << "Senegal is the winner of Group E" << endl;
        Q1groupE = senegal;
        Q1groupEattack = senegalattack;
        Q1groupEmidfield = senegalmidfield;
        Q1groupEdeffence = senegaldeffence;
        FQ1groupE = "Senegal";
    }
    else {}

     //group D
    
    //attack of wales
    if (walesattack > polandattack) {
        wales += 1;
    }
    if (walesattack > usaattack) {
        wales += 1;
    }
    if (walesattack > peruattack) {
        wales += 1;
    }

    //attack of poland
    if (polandattack > walesattack) {
        poland += 1;
    }
    if (polandattack > usaaattack) {
        poland += 1;
    }
    if (polandattack > peruattack) {
        poland += 1;
    }

    //attack of usa
    if (usaattack > walesattack) {
        usa += 1;
    }
    if (usaattack > polandattack) {
        usa += 1;
    }
    if (usaattack > peruattack) {
        usa += 1;
    }

    //attack of peru
    if (peruattack > usaattack) {
        peru += 1;
    }
    if (peruattack > polandattack) {
        peru += 1;
    }
    if (peruattack > walesattack) {
        peru += 1;
    }

    //midfield of wales
    if (walesmidfield > usamidfield) {
        wales += 1;
    }
    if (walesmidfield > polandmidfield) {
        wales += 1;
    }
    if (walesmidfield > perumidfield) {
        wales += 1;
    }

    //midfield of usa
    if (usamidfield > walesmidfield) {
        usa += 1;
    }
    if (usamidfield > polandmidfield) {
        usa += 1;
    }
    if (usamidfield > perumidfield) {
        usa += 1;
    } 

    //midfield of peru
    if (perumidfield > walesmidfield) {
        peru += 1;
    }
    if (perumidfield > usamidfield) {
        peru += 1;
    }
    if (perumidfield > polandmidfield) {
        peru += 1;
    } 

    //midfield of poland
    if (polandmidfield > walesmidfield) {
        poland += 1;
    }
    if (polandmidfield > usamidfield) {
        poland += 1;
    }
    if (polandmidfield > perusmidfield) {
        poland += 1;
    }
    
    //defense of wales
    if (walesdeffence > usadeffence) {
        wales += 1;
    }
    if (walesdeffence > polanddeffence) {
        wales += 1;
    }
    if (walesdeffence > perudeffence) {
        wales += 1;
    }

    //defense of usa
    if (usadeffence > polanddeffence) {
        usa += 1;
    }
    if (usadeffence > walesdeffence) {
        usa += 1;
    }
    if (usadeffence > perudeffence) {
        usa += 1;
    }

    //defense of poland
    if (polanddeffence > walesdeffence) {
        poland += 1;
    } 
    if (polanddeffence > usadeffence) {
        poland += 1;
    } 
    if (polanddeffence > perudeffence) {
        poland += 1;
    } 

    //defense of peru
    if (perudeffence > walesdeffence) {
        peru += 1;
    }
    if (perudeffence > usadeffence) {
        peru += 1;
    }
    if (perudeffence > polanddeffence) {
        peru += 1;
    }

    //1st place results of group D
     if (peru > wales && peru > usa && peru > poland) {
        cout << "Peru is the winner of Group D" << endl;
        Q1groupD = peru;
        Q1groupDattack = peruattack;
        Q1groupDmidfield = perumidfield;
        Q1groupDdeffence = perudeffence;
        FQ1groupD = "Peru";
    }
    else if (wales > peru && wales > usa && wales > poland) {
        cout << "Wales is the winner of Group D" << endl;
        Q1groupD = wales;
        Q1groupDattack = walesattack;
        Q1groupDmidfield = walesmidfield;
        Q1groupDdeffence = walesdeffence;
        FQ1groupD = "Wales";
    }
    else if (usa > wales && usa > peru && usa > poland) {
        cout << "USA is the winner of Group D" << endl;
        Q1groupD = usa;
        Q1groupDattack = usaattack;
        Q1groupDmidfield = usamidfield;
        Q1groupDdeffence = usadeffence;
        FQ1groupD = "USA";
    }
    else if (poland > wales && poland > peru && poland > usa) {
        cout << "Poland is the winner of Group D" << endl;
        Q1groupD = poland;
        Q1groupDattack = polandattack;
        Q1groupDmidfield = polandmidfield;
        Q1groupDdeffence = polanddeffence;
        FQ1groupD = "poland";
    }
    else {}

    //group C
    
    //attack of chile
    if (chileattack > swedenattack) {
        chile += 1;
    } 
    
    if (chileattack > netherlandsattack) {
        chile += 1;
    }
    
    if (chileattack > mexicoattack) {
        chile += 1;
    } 
    
    //attack of sweden
    if (swedenattack > chileattack) {
        sweden += 1;
    }
    
    if (swedenattack > netherlandsattack) {
        sweden += 1;
    } 
    
    if (swedenattack > mexicoattack) {
        sweden += 1;
    } 
     
    //attack of netherlands
    if (netherlandsattack > swedenattack) {
        netherlands += 1;
    }
     
     if (netherlandsattack > chileattack) {
        netherlands += 1;
    } 
    
    if (netherlandsattack > mexicoattack) {
        netherlands += 1;
    }
    
    
    //attack of mexico
    if (mexicoattack > chileattack) {
        mexico += 1;
    }
    
    if (mexicoattack > swedenattack) {
        mexico += 1;
    }
    
    if (mexicoattack > netherlandsattack) {
        mexico += 1;
    }
    
    //midfield of chile
    if (chilemidfield > swedenmidfield) {
        chile += 1;
    }
    
    if (chilemidfield > netherlandsmidfield) {
        chile += 1;
    }
    
    if (chilemidfield > mexicomidfield) {
        chile += 1;
    }
     
    //midfield of sweden
    if (swedenmidfield > chilemidfield) {
        sweden += 1;
    } 
    if (swedenmidfield > netherlandsmidfield) {
        sweden += 1;
    }
    if (swedenmidfield > mexicomidfield) {
        sweden += 1;
    }
    
    //midfield of netherlands
    if (netherlandsmidfield > chilemidfield) {
        netherlands += 1;
    }
    if (netherlandsmidfield > swedenmidfield) {
        netherlands += 1;
    }
    if (netherlandsmidfield > mexicomidfield) {
        netherlands += 1;
    } 
    
    //midfield of mexico 
    if (mexicomidfield > chilemidfield) {
        mexico += 1;
    }
    if (mexicomidfield > swedenmidfield) {
        mexico += 1;
    }
    if (mexicomidfield > netherlandsmidfield) {
        mexico += 1;
    }
    
    //defense of chile
    if (chiledeffence > swedendeffence) {
        chile += 1;
    }
    if (chiledeffence > netherlandsdeffence) {
        chile += 1;
    }
    if (chiledeffence > mexicodeffence) {
        chile += 1;
    }
     
     //defense of sweden
     if (swedendeffence > chiledeffence) {
         sweden += 1;
     }
     if (swedendeffence > netherlandsdeffence) {
         sweden += 1;
     }
     if (swedendeffence > mexicodeffence {
         sweden += 1;
     }
     
     //defense of netherlands
     if (netherlandsdeffence > chiledeffence) {
         netherlands += 1;
     }
     if (netherlandsdeffence > swedendeffence) {
         netherlands += 1;
     }
     if (netherlandsdeffence > mexicodeffence) {
         netherlands += 1;
     }
     
     //defense of mexico
     if (mexicodeffence > chiledeffence) {
         mexico += 1;
     }
     if (mexicodeffence > swedendeffence) {
         mexico += 1;
     }
     if (mexicodeffence > netherlandsdeffence) {
         mexico += 1;
     }

     //first place results of group C
     if (chile > netherlands && chile > sweden && chile > mexico) {
        cout << "Chile is the winner of Group C" << endl;
        Q1groupC = chile;
        Q1groupCattack = chileattack;
        Q1groupCmidfield = chilemidfield;
        Q1groupCdeffence = chiledeffence;
        FQ1groupC = "Chile";
        
    }
     else if (netherlands > chile && netherlands > sweden && netherlands > mexico) {
        cout << "Netherlands is the winner of Group C" << endl;
        Q1groupC = netherlands;
        Q1groupCattack = netherlandsattack;
        Q1groupCmidfield = netherlandsmidfield;
        Q1groupCdeffence = netherlandsdeffence;
        FQ1groupC = "Netherlands";
        
    }
    else if (sweden > chile && sweden > netherlands && sweden > mexico) {
        cout << "Sweden is the winner of Group C" << endl;
        Q1groupC = sweden;
        Q1groupCattack = swedenattack;
        Q1groupCmidfield = swedenmidfield;
        Q1groupCdeffence = swedendeffence;
        FQ1groupC = "Sweden";
        
    }
    else if (mexico > chile && mexico > sweden && mexico > netherlands) {
        cout << "Mexico is the winner of Group C" << endl;
        Q1groupC = mexico;
        Q1groupCattack = mexicoattack;
        Q1groupCmidfield = mexicomidfield;
        Q1groupCdeffence = mexicodeffence;
        FQ1groupC = "Mexico";
        
    }
    else {}
     
    //group B

    //attack of croatia
    if (croatiaattack > belgiumattack) {
        croatia += 1;
    }
    
    if (croatiaattack > denmarkattack) {
        croatia += 1;
    }

    if (croatiaattack > columbiaattack) {
        croatia += 1;
    }

    //attack of belgium
    if (belgiumattack > croatiaattack) {
        belgium += 1;
    }

    if (belgiumattack > denmarkattack) {
        belgium += 1;
    }

    if (belgiumattack > columbiaattack) {
        belgium += 1;
    }

    //attack of denmark
    if (denmarkattack > belgiumattack) {
        denmark += 1;
    }

    if (denmarkattack > croatiaattack) {
        denmark += 1;
    }

    if (denmarkattack > columbiaattack) {
        denmark += 1;
    }

    //attack of columbia
    if (columbiaattack > denmarkattack) {
        columbia += 1;
    }

    if (columbiaattack > belgiumattack) {
        columbia += 1;
    }

    if (columbiaattack > croatiaattack) {
        columbia += 1;
    }

    //midfield of croatia
    if (croatiamidfield > belgiummidfield) {
        croatia += 1;
    }
    
    if (croatiamidfield > denmarkmidfield) {
        croatia += 1;
    }

    if (croatiamidfield > columbiamidfield) {
        croatia += 1;
    }

    //midfield of belgium
    if (belgiummidfield > denmarkmidfield) {
        belgium += 1;
    }
    
    if (belgiummidfield > columbiamidfield) {
        belgium += 1;
    }

    if (belgiummidfield > croatiamidfield) {
        belgium += 1;
    }

    //midfield of denmark
    if (denmarkmidfield > columbiamidfield) {
        denmark += 1;
    }
    
    if (denmarkmidfield > croatiamidfield) {
        denmark += 1;
    }

    if (denmarkmidfield > belgiummidfield) {
        denmark += 1;
    }

    //midfield of columbia
    if (columbiamidfield > denmarkmidfield) {
        columbia += 1;
    }
    
    if (columbiamidfield > croatiamidfield) {
        columbia += 1;
    }

    if (columbiamidfield > belgiummidfield) {
        columbia += 1;
    }

    //deffence of denmark
    if (denmarkdeffence > croatiadeffence) {
        denmark += 1;
    }
    
    if (denmarkdeffence > belgiumdeffence) {
        denmark += 1;
    }

    if (denmarkdeffence > columbiadeffence) {
        denmark += 1;
    }

    //deffence of croatia
    if (croatiadeffence > columbiadeffence) {
        croatia += 1;
    }
    
    if (croatiadeffence > belgiumdeffence) {
        croatia += 1;
    }

    if (croatiadeffence > denmarkdeffence) {
        croatia += 1;
    }
    
    //deffence of belgium
    if (belgiumdeffence > denmarkdeffence) {
        belgium += 1;
    }
    
    if (belgiumdeffence > croatiadeffence) {
        belgium += 1;
    }

    if (belgiumdeffence > columbiadeffence) {
        belgium += 1;
    }

    //deffence of columbia
    if (columbiadeffence > belgiumdeffence) {
        columbia += 1;
    }
    
    if (columbiadeffence > croatiadeffence) {
        columbia += 1;
    }

    if (columbiadeffence > denmarkdeffence) {
        columbia += 1;
    }

    //1st place results of group B
    if (columbia > denmark && columbia > croatia && columbia > belgium) {
        cout << "Columbia is the winner of Group B" << endl;
        Q1groupB = columbia;
        Q1groupBattack = columbiaattack;
        Q1groupBmidfield = columbiamidfield;
        Q1groupBdeffence = columbiadeffence;
        FQ1groupB = "Columbia";
        
    }

    else if (denmark > columbia && denmark > croatia && denmark > belgium) {
        cout << "Denmark is the winner of Group B" << endl;
        Q1groupB = denmark;
        Q1groupBattack = denmarkattack;
        Q1groupBmidfield = denmarkmidfield;
        Q1groupBdeffence = denmarkdeffence;
        FQ1groupB = "Denmark";
        
    }

    else if (croatia > denmark && croatia > belgium && croatia > columbia) {
        cout << "Croatia is the winner of Group B" << endl;
        Q1groupB = croatia;
        Q1groupBattack = croatiaattack;
        Q1groupBmidfield = croatiamidfield;
        Q1groupBdeffence = croatiadeffence;
        FQ1groupB = "Croatia";
        
    }

    else if (belgium > denmark && belgium > croatia && belgium > columbia) {
        cout << "Belgium is the winner of Group B" << endl;
        Q1groupB = belgium;
        Q1groupBattack = belgiumattack;
        Q1groupBmidfield = belgiummidfield;
        Q1groupBdeffence = belgiumdeffence;
        FQ1groupB = "Belgium";
        
    }

    else {}

    //2nd place results
   
    //Columbia
    if (columbia > denmark && columbia > croatia && columbia < belgium) {
        cout << "Columbia is the second of Group B" << endl;
        Q2groupB = columbia;
        Q2groupBattack = columbiaattack;
        Q2groupBmidfield = columbiamidfield;
        Q2groupBdeffence = columbiadeffence;
        FQ2groupB = "Columbia";
        FR1game1F = "Columbia";
        FR1game1T = "Columbia";
    }

    else if (columbia > denmark && columbia < croatia && columbia > belgium) {
        cout << "Columbia is the second of Group B" << endl;
        Q2groupB = columbia;
        Q2groupBattack = columbiaattack;
        Q2groupBmidfield = columbiamidfield;
        Q2groupBdeffence = columbiadeffence;
        FQ2groupB = "Columbia";
        FR1game1F = "Columbia";
        FR1game1T = "Columbia";
    }

    else if (columbia < denmark && columbia > croatia && columbia > belgium) {
        cout << "Columbia is the second of Group B" << endl;
        Q2groupB = columbia;
        Q2groupBattack = columbiaattack;
        Q2groupBmidfield = columbiamidfield;
        Q2groupBdeffence = columbiadeffence;
        FQ2groupB = "Columbia";
        FR1game1F = "Columbia";
        FR1game1T = "Columbia";
    }

    else {}

    //Denmark
    if (denmark > columbia && denmark > croatia && denmark < belgium) {
        cout << "Denmark is the second of Group B" << endl;
        Q2groupB = denmark;
        Q2groupBattack = denmarkattack;
        Q2groupBmidfield = denmarkmidfield;
        Q2groupBdeffence = denmarkdeffence;
        FQ2groupB = "Denmark";
        FR1game1F = "Denmark";
        FR1game1T = "Denmark";
    }

    else if (denmark > columbia && denmark < croatia && denmark > belgium) {
        cout << "Denmark is the second of Group B" << endl;
        Q2groupB = denmark;
        Q2groupBattack = denmarkattack;
        Q2groupBmidfield = denmarkmidfield;
        Q2groupBdeffence = denmarkdeffence;
        FQ2groupB = "Denmark";
        FR1game1F = "Denmark";
        FR1game1T = "Denmark";
    }

    else if (denmark < columbia && denmark > croatia && denmark > belgium) {
        cout << "Denmark is the second of Group B" << endl;
        Q2groupB = denmark;
        Q2groupBattack = denmarkattack;
        Q2groupBmidfield = denmarkmidfield;
        Q2groupBdeffence = denmarkdeffence;
        FQ2groupB = "Denmark";
        FR1game1F = "Denmark";
        FR1game1T = "Denmark";
    }

    else {}

    //Croatia
    if (croatia > denmark && croatia > belgium && croatia < columbia) {
        cout << "Croatia is the second of Group B" << endl;
        Q2groupB = croatia;
        Q2groupBattack = croatiaattack;
        Q2groupBmidfield = croatiamidfield;
        Q2groupBdeffence = croatiadeffence;
        FQ2groupB = "Croatia";
        FR1game1F = "Croatia";
        FR1game1T = "Croatia";
    }

    else if (croatia > denmark && croatia < belgium && croatia > columbia) {
        cout << "Croatia is the second of Group B" << endl;
        Q2groupB = croatia;
        Q2groupBattack = croatiaattack;
        Q2groupBmidfield = croatiamidfield;
        Q2groupBdeffence = croatiadeffence;
        FQ2groupB = "Croatia";
        FR1game1F = "Croatia";
        FR1game1T = "Croatia";
    }

    else if (croatia < denmark && croatia > belgium && croatia > columbia) {
        cout << "Croatia is the second of Group B" << endl;
        Q2groupB = croatia;
        Q2groupBattack = croatiaattack;
        Q2groupBmidfield = croatiamidfield;
        Q2groupBdeffence = croatiadeffence;
        FQ2groupB = "Croatia";
        FR1game1F = "Croatia";
        FR1game1T = "Croatia";
    }

    else {}

    //Belgium
    if (belgium > denmark && belgium > croatia && belgium < columbia) {
        cout << "Belgium is the second of Group B" << endl;
        Q2groupB = belgium;
        Q2groupBattack = belgiumattack;
        Q2groupBmidfield = belgiummidfield;
        Q2groupBdeffence = belgiumdeffence;
        FQ2groupB = "Belgium";
        FR1game1F = "Belgium";
        FR1game1T = "Belgium";
    }

    else if (belgium > denmark && belgium < croatia && belgium > columbia) {
        cout << "Belgium is  the second of Group B" << endl;
        Q2groupB = belgium;
        Q2groupBattack = belgiumattack;
        Q2groupBmidfield = belgiummidfield;
        Q2groupBdeffence = belgiumdeffence;
        FQ2groupB = "Belgium";
        FR1game1F = "Belgium";
        FR1game1T = "Belgium";
    }

    else if (belgium < denmark && belgium > croatia && belgium > columbia) {
        cout << "Belgium is the second of Group B" << endl;
        Q2groupB = belgium;
        Q2groupBattack = belgiumattack;
        Q2groupBmidfield = belgiummidfield;
        Q2groupBdeffence = belgiumdeffence;
        FQ2groupB = "Belgium";
        FR1game1F = "Belgium";
        FR1game1T = "Belgium";
    }

    else {}

    cout << endl;

    //@@@@@@@@@@@@@@

    //group A

    //attack of italy
    if (italyattack > portugalattack) {
        italy += 1;
    }
    
    if (italyattack > australiaattack) {
        italy += 1;
    }

    if (italyattack > iranattack) {
        italy += 1;
    }

    //attack of portugal
    if (portugalattack > italyattack) {
        portugal += 1;
    }

    if (portugalattack > australiaattack) {
        portugal += 1;
    }

    if (portugalattack > iranattack) {
        portugal += 1;
    }

    //attack of australia
    if (australiaattack > italyattack) {
        australia += 1;
    }

    if (australiaattack > portugalattack) {
        australia += 1;
    }

    if (australiaattack > iranattack) {
        australia += 1;
    }

    //attack of iran
    if (iranattack > italyattack) {
        iran += 1;
    }

    if (iranattack > portugalattack) {
        iran += 1;
    }

    if (iranattack > australiaattack) {
        iran += 1;
    }

    //midfield of italy
    if (italymidfield > portugalmidfield) {
        italy += 1;
    }
    
    if (italymidfield > australiamidfield) {
        italy += 1;
    }

    if (italymidfield > iranmidfield) {
        italy += 1;
    }

    //midfield of portugal
    if (portugalmidfield > italymidfield) {
        portugal += 1;
    }
    
    if (portugalmidfield > australiamidfield) {
        portugal += 1;
    }

    if (portugalmidfield > iranmidfield) {
        portugal += 1;
    }

    //midfield of australia
    if (australiamidfield > italymidfield) {
        australia += 1;
    }
    
    if (australiamidfield > portugalmidfield) {
        australia += 1;
    }

    if (australiamidfield > iranmidfield) {
        australia += 1;
    }

    //midfield of iran
    if (iranmidfield > italymidfield) {
        iran += 1;
    }
    
    if (iranmidfield > portugalmidfield) {
        iran += 1;
    }

    if (iranmidfield > australiamidfield) {
        iran += 1;
    }

    //deffence of italy
    if (italydeffence > portugaldeffence) {
        italy += 1;
    }
    
    if (italydeffence > australiadeffence) {
        italy += 1;
    }

    if (italydeffence > irandeffence) {
        italy += 1;
    }

    //deffence of portugal
    if (portugaldeffence > italydeffence) {
        portugal += 1;
    }
    
    if (portugaldeffence > australiadeffence) {
        portugal += 1;
    }

    if (portugaldeffence > irandeffence) {
        portugal += 1;
    }
    
    //deffence of australia
    if (australiadeffence > italydeffence) {
        australia += 1;
    }
    
    if (australiadeffence > portugaldeffence) {
        australia += 1;
    }

    if (australiadeffence > irandeffence) {
        australia += 1;
    }

    //deffence of iran
    if (irandeffence > italydeffence) {
        iran += 1;
    }
    
    if (irandeffence > portugaldeffence) {
        iran += 1;
    }

    if (irandeffence > australiadeffence) {
        iran += 1;
    }

    //1st place results
    if (italy > portugal && italy > australia && italy > iran) {
        cout << "Italy is the winner of Group A" << endl;
        Q1groupA = italy;
        Q1groupAattack = italyattack;
        Q1groupAmidfield = italymidfield;
        Q1groupAdeffence = italydeffence;
        FQ1groupA = "Italy";
        
    }

    else if (portugal > italy && portugal > australia && portugal > iran) {
        cout << "Portugal is the winner of Group A" << endl;
        Q1groupA = portugal;
        Q1groupAattack = portugalattack;
        Q1groupAmidfield = portugalmidfield;
        Q1groupAdeffence = portugaldeffence;
        FQ1groupA = "Portugal";
        FR1game1F = "Portugal";
        FR1game1T = "Portugal";
    }

    else if (australia > italy && australia > portugal && australia > iran) {
        cout << "Australia is the winner of Group A" << endl;
        Q1groupA = australia;
        Q1groupAattack = australiaattack;
        Q1groupAmidfield = australiamidfield;
        Q1groupAdeffence = australiadeffence;
        FQ1groupA = "Australia";
        FR1game1F = "Australia";
        FR1game1T = "Australia";
    }

    else if (iran > italy && iran > portugal && iran > australia) {
        cout << "Iran is the winner of Group A" << endl;
        Q1groupA = iran;
        Q1groupAattack = iranattack;
        Q1groupAmidfield = iranmidfield;
        Q1groupAdeffence = irandeffence;
        FQ1groupA = "Iran";
        FR1game1F = "Iran";
        FR1game1T = "Iran";
    }

    else {}

    //2nd place results
   
    //Italy
    if (italy > portugal && italy > australia && italy < iran) {
        cout << "Italy is the second of Group A" << endl;
        Q2groupA = italy;
        Q2groupAattack = italyattack;
        Q2groupAmidfield = italymidfield;
        Q2groupAdeffence = italydeffence;
        FQ2groupA = "Italy";
        FR1game2F = "Italy";
        FR1game2T = "Italy";
    }

    else if (italy > portugal && italy < australia && italy > iran) {
        cout << "Italy is the second of Group A" << endl;
        Q2groupA = italy;
        Q2groupAattack = italyattack;
        Q2groupAmidfield = italymidfield;
        Q2groupAdeffence = italydeffence;
        FQ2groupA = "Italy";
        FR1game2F = "Italy";
        FR1game2T = "Italy";
    }

    else if (italy < portugal && italy > australia && italy > iran) {
        cout << "Italy is the second of Group A" << endl;
        Q2groupA = italy;
        Q2groupAattack = italyattack;
        Q2groupAmidfield = italymidfield;
        Q2groupAdeffence = italydeffence;
        FQ2groupA = "Italy";
        FR1game2F = "Italy";
        FR1game2T = "Italy";
    }

    else {}

    //Portugal
    if (portugal > italy && portugal > australia && portugal < iran) {
        cout << "Portugal is the second of Group A" << endl;
        Q2groupA = portugal;
        Q2groupAattack = portugalattack;
        Q2groupAmidfield = portugalmidfield;
        Q2groupAdeffence = portugaldeffence;
        FQ2groupA = "Portugal";
        FR1game2F = "Portugal";
        FR1game2T = "Portugal";
    }

    else if (portugal > italy && portugal < australia && portugal > iran) {
        cout << "Portugal is the second of Group A" << endl;
        Q2groupA = portugal;
        Q2groupAattack = portugalattack;
        Q2groupAmidfield = portugalmidfield;
        Q2groupAdeffence = portugaldeffence;
        FQ2groupA = "Portugal";
        FR1game2F = "Portugal";
        FR1game2T = "Portugal";
    }

    else if (portugal < italy && portugal > australia && portugal > iran) {
        cout << "Portugal is the second of Group A" << endl;
        Q2groupA = portugal;
        Q2groupAattack = portugalattack;
        Q2groupAmidfield = portugalmidfield;
        Q2groupAdeffence = portugaldeffence;
        FQ2groupA = "Portugal";
        FR1game2F = "Portugal";
        FR1game2T = "Portugal";
    }

    else {}

    //Australia
    if (australia > italy && australia > portugal && australia < iran) {
        cout << "Australia is the second of Group A" << endl;
        Q2groupA = australia;
        Q2groupAattack = australiaattack;
        Q2groupAmidfield = australiamidfield;
        Q2groupAdeffence = australiadeffence;
        FQ2groupA = "Australia";
        FR1game2F = "Australia";
        FR1game2T = "Australia";
    }

    else if (australia > italy && australia < portugal && australia > iran) {
        cout << "Australia is the second of Group A" << endl;
        Q2groupA = australia;
        Q2groupAattack = australiaattack;
        Q2groupAmidfield = australiamidfield;
        Q2groupAdeffence = australiadeffence;
        FQ2groupA = "Australia";
        FR1game2F = "Australia";
        FR1game2T = "Australia";
    }

    else if (australia < italy && australia > portugal && australia > iran) {
        cout << "Australia is the second of Group A" << endl;
        Q2groupA = australia;
        Q2groupAattack = australiaattack;
        Q2groupAmidfield = australiamidfield;
        Q2groupAdeffence = australiadeffence;
        FQ2groupA = "Australia";
        FR1game2F = "Australia";
        FR1game2T = "Australia";
    }

    else {}

    //Iran
    if (iran > italy && iran > portugal && iran < australia) {
        cout << "Iran is the second of Group A" << endl;
        Q2groupA = iran;
        Q2groupAattack = iranattack;
        Q2groupAmidfield = iranmidfield;
        Q2groupAdeffence = irandeffence;
        FQ2groupA = "Iran";
        FR1game2F = "Iran";
        FR1game2T = "Iran";
    }

    else if (iran > italy && iran < portugal && iran > australia) {
        cout << "Iran is the second of Group A" << endl;
        Q2groupA = iran;
        Q2groupAattack = iranattack;
        Q2groupAmidfield = iranmidfield;
        Q2groupAdeffence = irandeffence;
        FQ2groupA = "Iran";
        FR1game2F = "Iran";
        FR1game2T = "Iran";
    }

    else if (iran < italy && iran > portugal && iran > australia) {
        cout << "Iran is the second of Group A" << endl;
        Q2groupA = iran;
        Q2groupAattack = iranattack;
        Q2groupAmidfield = iranmidfield;
        Q2groupAdeffence = irandeffence;
        FQ2groupA = "Iran";
        FR1game2F = "Iran";
        FR1game2T = "Iran";
    }

    else {}
    
    //Qualification matches
    
    //Qualified teams' attack, midfield, deffence difference
    
    //Game one's comparison
    //Attack
    if (Q1groupAattack > Q2groupBattack) {
        Q1groupA += 1;
    }

    else if (Q1groupAattack < Q2groupBattack) {
        Q2groupB += 1;
    }

    //midfield
    if (Q1groupAmidfield > Q2groupBmidfield) {
        Q1groupA += 1;
    }

    else if (Q1groupAmidfield < Q2groupBmidfield) {
        Q2groupB += 1;
    }

    //deffence
    if (Q1groupAdeffence > Q2groupBdeffence) {
        Q1groupA += 1;
    }

    else if (Q1groupAdeffence < Q2groupBdeffence) {
        Q2groupB += 1;
    }

    //Game two's comparison
    //Attack
    if (Q1groupBattack > Q2groupAattack) {
        Q1groupB += 1;
    }

    else if (Q1groupBattack < Q2groupAattack) {
        Q2groupA += 1;
    }

    //midfield
    if (Q1groupBmidfield > Q2groupAmidfield) {
        Q1groupB += 1;
    }

    else if (Q1groupBmidfield < Q2groupAmidfield) {
        Q2groupA += 1;
    }

    //deffence
    if (Q1groupBdeffence > Q2groupAdeffence) {
        Q1groupB += 1;
    }

    else if (Q1groupBdeffence < Q2groupAdeffence) {
        Q2groupA += 1;
    }

    cout << endl;
    
    //Round 1 match results
    //game 1
    if (Q1groupA > Q2groupB) {
        cout << FQ1groupA <<" won "<< FQ2groupB << " in round 1" << endl;
        R1game1F = Q1groupA;
        R1game1Fattack = Q1groupAattack;
        R1game1Fmidfield = Q1groupAmidfield;
        R1game1Fdeffence = Q1groupAdeffence;
        R1game1T = Q2groupB;
        R1game1Tattack = Q2groupBattack;
        R1game1Tmidfield = Q2groupBmidfield;
        R1game1Tdeffence = Q2groupBdeffence;
    }

    if (Q1groupA < Q2groupB) {
        cout << FQ2groupB <<" won "<< FQ1groupA << " in round 1" << endl;
        R1game1F = Q2groupB;
        R1game1Fattack = Q2groupBattack;
        R1game1Fmidfield = Q2groupBmidfield;
        R1game1Fdeffence = Q2groupBdeffence;
        R1game1T = Q1groupA;
        R1game1Tattack = Q1groupAattack;
        R1game1Tmidfield = Q1groupAmidfield;
        R1game1Tdeffence = Q1groupAdeffence;
    }

    //game 2
    if (Q2groupA > Q1groupB) {
        cout << FQ2groupA <<" won "<< FQ1groupB << " in round 1" << endl;
        R1game2F = Q2groupA;
        R1game2Fattack = Q2groupAattack;
        R1game2Fmidfield = Q2groupAmidfield;
        R1game2Fdeffence = Q2groupAdeffence;
        R1game2T = Q1groupB;
        R1game2Tattack = Q1groupBattack;
        R1game2Tmidfield = Q1groupBmidfield;
        R1game2Tdeffence = Q1groupBdeffence;
    }

    if (Q2groupA < Q1groupB) {
        cout << FQ1groupB <<" won "<< FQ2groupA << " in round 1" << endl;
        R1game2F = Q1groupB;
        R1game2Fattack = Q1groupBattack;
        R1game2Fmidfield = Q1groupBmidfield;
        R1game2Fdeffence = Q1groupBdeffence;
        R1game2T = Q2groupA;
        R1game2Tattack = Q2groupAattack;
        R1game2Tmidfield = Q2groupAmidfield;
        R1game2Tdeffence = Q2groupAdeffence;
    }
    
    
    //Comparison of finals teams' attack
    if (R1game1Fattack > R1game2Fattack) {
        R1game1F += 1;
    }

    else if (R1game1Fattack < R1game2Fattack) {
        R1game2F += 1;
    }

    //Comparison of finals teams' midfield
    if (R1game1Fmidfield > R1game2Fmidfield) {
        R1game1F += 1;
    }

    else if (R1game1Fmidfield < R1game2Fmidfield) {
        R1game2F += 1;
    }

    //Comparison of finals teams' defence
    if (R1game1Fdeffence > R1game2Fdeffence) {
        R1game1F += 1;
    }

    else if (R1game1Fdeffence < R1game2Fdeffence) {
        R1game2F += 1;
    }

    //Comparison of third place game's teams' attack
    if (R1game1Tattack > R1game2Tattack) {
        R1game1T += 1;
    }

    else if (R1game1Tattack < R1game2Tattack) {
        R1game2T += 1;
    }

    //Comparison of third place game's teams' midfield
    if (R1game1Tmidfield > R1game2Tmidfield) {
        R1game1T += 1;
    }

    else if (R1game1Tmidfield < R1game2Tmidfield) {
        R1game2T += 1;
    }

    //Comparison of third place game's teams' defence
    if (R1game1Tdeffence > R1game2Tdeffence) {
        R1game1T += 1;
    }

    else if (R1game1Tdeffence < R1game2Tdeffence) {
        R1game2T += 1;
    }

    cout << endl;

    //Third Place
    if (R1game1T > R1game2T) {
       cout << FR1game1T << " are the third place winners";
    }

    else if (R1game1T < R1game2T) {
       cout << FR1game2T << " are the third place winners";
    }

    cout << endl;

    //Finals
    if (R1game1F > R1game2F) {
       cout << FR1game1F << " are the World Cup Champions!!!!!!!!!!!!!!!!!!!!!!!!!!!";
    }

    else if (R1game1F < R1game2F) {
       cout << FR1game2F << " are the World Cup Champions!!!!!!!!!!!!!!!!!!!!!!!!!!!";
    }
    
    























}
