//CS FINAL PROJECT: SOCCER WORLD CUP SIMULATOR
//MADE BY: APOORV JOSHI AND BEHZOD TOJIEV
//CLASS: CS 171-3
//INSTRUCTOR: SCOTT GRIFFITH

////////////////////////////////////////////////////////////////////////////////////////


// This is a world cup simulator consisting of 32 teams and 8 groups


#include <iostream> //Output cout
#include <cstdlib>
#include <ctime> //Used to generate random numbers very time the code is run
using namespace std;

int main () { //the main function

    srand(time(NULL));  

    //Random number generator for unexpected factors. As it adds random numbers from 0-9 to the original in the unexpected factors section
   // These have 32 ints for 32 teams
    int r1 = rand() % 10;
    int r2 = rand() % 10;
    int r3 = rand() % 10;
    int r4 = rand() % 10;
    int r5 = rand() % 10;
    int r6 = rand() % 10;
    int r7 = rand() % 10;
    int r8 = rand() % 10;
    int r9 = rand() % 10;
    int r10 = rand() % 10;
    int r11 = rand() % 10;
    int r12 = rand() % 10;
    int r13 = rand() % 10;
    int r14 = rand() % 10;
    int r15 = rand() % 10;
    int r16 = rand() % 10;
    int r17 = rand() % 10;
    int r18 = rand() % 10;
    int r19 = rand() % 10;
    int r20 = rand() % 10;
    int r21 = rand() % 10;
    int r22 = rand() % 10;
    int r23 = rand() % 10;
    int r24 = rand() % 10;
    int r25 = rand() % 10;
    int r26 = rand() % 10;
    int r27 = rand() % 10;
    int r28 = rand() % 10;
    int r29 = rand() % 10;
    int r30 = rand() % 10;
    int r31 = rand() % 10;
    int r32 = rand() % 10;
    
    //Every team has its own game type. It will go through group stages, then to quater finals, then to semi finals, and then the finals
    //Here, we designed the base of the code by defining every country/team using string. For example 'string FR1game1F' means that the team
    //is in the final round of the world cup and will compete with 'string FR1game2F' in the final round.
    

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

    //Semi-Finals
    int SFgame1;
    int SFgame2;
    int SFgame3;
    int SFgame4;
    string FSFgame1;
    string FSFgame2;
    string FSFgame3;
    string FSFgame4;

    //Quarter-Finals
    int QFgame1;
    int QFgame2;
    int QFgame3;
    int QFgame4;
    int QFgame5;
    int QFgame6;
    int QFgame7;
    int QFgame8;
    string FQFgame1;
    string FQFgame2;
    string FQFgame3;
    string FQFgame4;
    string FQFgame5;
    string FQFgame6;
    string FQFgame7;
    string FQFgame8;

    //Qualified teams
    
    //Qulified in 1st place from group A
    int Q1groupA;
    string FQ1groupA;

    //Qualified in 2nd place from group A
    int Q2groupA;
    string FQ2groupA;

    //Qulified in 1st place from group B
    int Q1groupB;
    string FQ1groupB;

    //Qualified in 2nd place from group B
    int Q2groupB;
    string FQ2groupB;

    //Qualified in 1st place from group C
    int Q1groupC;
    string FQ1groupC;

    //Qualified in 2nd place from group C
    int Q2groupC;
    string FQ2groupC;

    //Qualified in 1st place from group D
    int Q1groupD;
    string FQ1groupD;

    //Qualified in 2nd place from group D
    int Q2groupD;
    string FQ2groupD;

    //Qualified in 1st place from group E
    int Q1groupE;
    string FQ1groupE;

    //Qualified in 2nd place from group E
    int Q2groupE;
    string FQ2groupE;

    //Qualified in 1st place from group F
    int Q1groupF;
    string FQ1groupF;

    //Qualified in 2nd place from group F
    int Q2groupF;
    string FQ2groupF;

    //Qulified in 1st place from group G
    int Q1groupG;
    string FQ1groupG;

    //Qualified in 2nd place from group G
    int Q2groupG;
    string FQ2groupG;

    //Qulified in 1st place from group H
    int Q1groupH;
    string FQ1groupH;

    //Qualified in 2nd place from group H
    int Q2groupH;
    string FQ2groupH;
    
    //We have defined int for every team having their own individual factors andn the compiler will compare a team's factor and then will
    // output which team won in which round. These are all the groups and their factors defined
    
    //Qualified teams' attack, midfield, deffence, factor of unexpectancy, currency in Euros, popuplation, # of goals score in last 5 games, # of goals conceded in last 5 games, # of victories in last 5 games, # of defeats in last 5 games of round 1
    int Q1groupAattack, Q1groupBattack, Q1groupCattack, Q1groupDattack, Q1groupEattack, Q1groupFattack, Q1groupGattack, Q1groupHattack, Q2groupAattack, Q2groupBattack, Q2groupCattack, Q2groupDattack, Q2groupEattack, Q2groupFattack, Q2groupGattack, Q2groupHattack;
    int Q1groupAmidfield, Q1groupBmidfield, Q1groupCmidfield, Q1groupDmidfield, Q1groupEmidfield, Q1groupFmidfield, Q1groupGmidfield, Q1groupHmidfield, Q2groupAmidfield, Q2groupBmidfield, Q2groupCmidfield, Q2groupDmidfield, Q2groupEmidfield, Q2groupFmidfield, Q2groupGmidfield, Q2groupHmidfield;
    int Q1groupAdeffence, Q1groupBdeffence, Q1groupCdeffence, Q1groupDdeffence, Q1groupEdeffence, Q1groupFdeffence, Q1groupGdeffence, Q1groupHdeffence, Q2groupAdeffence, Q2groupBdeffence, Q2groupCdeffence, Q2groupDdeffence, Q2groupEdeffence, Q2groupFdeffence, Q2groupGdeffence, Q2groupHdeffence;
    int Q1groupAf, Q1groupBf, Q1groupCf, Q1groupDf, Q1groupEf, Q1groupFf, Q1groupGf, Q1groupHf, Q2groupAf, Q2groupBf, Q2groupCf, Q2groupDf, Q2groupEf, Q2groupFf, Q2groupGf, Q2groupHf;
    int Q1groupAcost, Q1groupBcost, Q1groupCcost, Q1groupDcost, Q1groupEcost, Q1groupFcost, Q1groupGcost, Q1groupHcost, Q2groupAcost, Q2groupBcost, Q2groupCcost, Q2groupDcost, Q2groupEcost, Q2groupFcost, Q2groupGcost, Q2groupHcost;
    int Q1groupApop, Q1groupBpop, Q1groupCpop, Q1groupDpop, Q1groupEpop, Q1groupFpop, Q1groupGpop, Q1groupHpop, Q2groupApop, Q2groupBpop, Q2groupCpop, Q2groupDpop, Q2groupEpop, Q2groupFpop, Q2groupGpop, Q2groupHpop;
    int Q1groupA5, Q1groupB5, Q1groupC5, Q1groupD5, Q1groupE5, Q1groupF5, Q1groupG5, Q1groupH5, Q2groupA5, Q2groupB5, Q2groupC5, Q2groupD5, Q2groupE5, Q2groupF5, Q2groupG5, Q2groupH5;
    int Q1groupAC5, Q1groupBC5, Q1groupCC5, Q1groupDC5, Q1groupEC5, Q1groupFC5, Q1groupGC5, Q1groupHC5, Q2groupAC5, Q2groupBC5, Q2groupCC5, Q2groupDC5, Q2groupEC5, Q2groupFC5, Q2groupGC5, Q2groupHC5;
    int Q1groupAV5, Q1groupBV5, Q1groupCV5, Q1groupDV5, Q1groupEV5, Q1groupFV5, Q1groupGV5, Q1groupHV5, Q2groupAV5, Q2groupBV5, Q2groupCV5, Q2groupDV5, Q2groupEV5, Q2groupFV5, Q2groupGV5, Q2groupHV5;
    int Q1groupAD5, Q1groupBD5, Q1groupCD5, Q1groupDD5, Q1groupED5, Q1groupFD5, Q1groupGD5, Q1groupHD5, Q2groupAD5, Q2groupBD5, Q2groupCD5, Q2groupDD5, Q2groupED5, Q2groupFD5, Q2groupGD5, Q2groupHD5;
    
    //Quarter-finals teams' attack, midfield, deffence, factor of unexpectancy, currency in Euros, popuplation, # of goals score in last 5 games, # of goals conceded in last 5 games, # of victories in last 5 games, # of defeats in last 5 games
    int QFgame1attack, QFgame2attack, QFgame3attack, QFgame4attack, QFgame5attack, QFgame6attack, QFgame7attack, QFgame8attack;
    int QFgame1midfield, QFgame2midfield, QFgame3midfield, QFgame4midfield, QFgame5midfield, QFgame6midfield, QFgame7midfield, QFgame8midfield;
    int QFgame1deffence, QFgame2deffence, QFgame3deffence, QFgame4deffence, QFgame5deffence, QFgame6deffence, QFgame7deffence, QFgame8deffence;
    int QFgame1f, QFgame2f, QFgame3f, QFgame4f, QFgame5f, QFgame6f, QFgame7f, QFgame8f;
    int QFgame1cost, QFgame2cost, QFgame3cost, QFgame4cost, QFgame5cost, QFgame6cost, QFgame7cost, QFgame8cost;
    int QFgame1pop, QFgame2pop, QFgame3pop, QFgame4pop, QFgame5pop, QFgame6pop, QFgame7pop, QFgame8pop;
    int QFgame15, QFgame25, QFgame35, QFgame45, QFgame55, QFgame65, QFgame75, QFgame85;
    int QFgame1C5, QFgame2C5, QFgame3C5, QFgame4C5, QFgame5C5, QFgame6C5, QFgame7C5, QFgame8C5;
    int QFgame1V5, QFgame2V5, QFgame3V5, QFgame4V5, QFgame5V5, QFgame6V5, QFgame7V5, QFgame8V5;
    int QFgame1D5, QFgame2D5, QFgame3D5, QFgame4D5, QFgame5D5, QFgame6D5, QFgame7D5, QFgame8D5;

    //Semi-finals teams' attack, midfield, deffence, factor of unexpectancy, currency in Euros, popuplation, # of goals score in last 5 games, # of goals conceded in last 5 games, # of victories in last 5 games, # of defeats in last 5 games
    int SFgame1attack, SFgame2attack, SFgame3attack, SFgame4attack;
    int SFgame1midfield, SFgame2midfield, SFgame3midfield, SFgame4midfield;
    int SFgame1deffence, SFgame2deffence, SFgame3deffence, SFgame4deffence;
    int SFgame1f, SFgame2f, SFgame3f, SFgame4f;
    int SFgame1cost, SFgame2cost, SFgame3cost, SFgame4cost;
    int SFgame1pop, SFgame2pop, SFgame3pop, SFgame4pop;
    int SFgame15, SFgame25, SFgame35, SFgame45;
    int SFgame1C5, SFgame2C5, SFgame3C5, SFgame4C5;
    int SFgame1V5, SFgame2V5, SFgame3V5, SFgame4V5;
    int SFgame1D5, SFgame2D5, SFgame3D5, SFgame4D5;

    //Finals teams' attack, midfield, deffence, factor of unexpectancy, currency in Euros, popuplation, # of goals score in last 5 games, # of goals conceded in last 5 games, # of victories in last 5 games, # of defeats in last 5 games
    int R1game1Fattack, R1game2Fattack;
    int R1game1Fmidfield, R1game2Fmidfield;
    int R1game1Fdeffence, R1game2Fdeffence;
    int R1game1Ff, R1game2Ff;
    int R1game1Fcost, R1game2Fcost;
    int R1game1Fpop, R1game2Fpop;
    int R1game1F5, R1game2F5;
    int R1game1FC5, R1game2FC5;
    int R1game1FV5, R1game2FV5;
    int R1game1FD5, R1game2FD5;

    //Match for third place teams' attack, midfield, deffence, factor of unexpectancy, currency in Euros, popuplation, # of goals score in last 5 games, # of goals conceded in last 5 games, # of victories in last 5 games, # of defeats in last 5 games
    int R1game1Tattack, R1game2Tattack;
    int R1game1Tmidfield, R1game2Tmidfield;
    int R1game1Tdeffence, R1game2Tdeffence;
    int R1game1Tf, R1game2Tf;
    int R1game1Tcost, R1game2Tcost;
    int R1game1Tpop, R1game2Tpop;
    int R1game1T5, R1game2T5;
    int R1game1TC5, R1game2TC5;
    int R1game1TV5, R1game2TV5;
    int R1game1TD5, R1game2TD5;


    //We now start with 8 groups from group A to group H, defining every factors of a particular country
    //All the statistics of a particular team has been taken from the internet.


    //group A (Italy, Portugal, Australia, Iran)

    int portugal = 0, italy = 0, australia = 0, iran = 0;
    
    //attack
    int italyattack = 90;
    int portugalattack = 82;
    int australiaattack = 85;
    int iranattack = 81;

    //midfield
    int italymidfield = 92;
    int portugalmidfield = 83;
    int australiamidfield = 81;
    int iranmidfield = 83;

    //defense
    int italydeffence = 85;
    int portugaldeffence = 81;
    int australiadeffence = 79;
    int irandeffence = 75;

    //factor of unexpectancy
    int fportugal = rand() % 100;
    int fitaly = rand() % 100;
    int faustralia = rand() % 100;
    int firan = rand() % 100;
    
    //currency in Euros
    double italycost = 426000000;
    double portugalcost = 466000000;
    double australiacost = 46000000;
    double irancost = 43000000;

    //popuplation
    double italypop = 59257878;
    double portugalpop = 10274947;
    double australiapop = 24912343;
    double iranpop = 24912343;

    //# of goals score in last 5 games
    int italy5 = 3;
    int portugal5 = 8;
    int australia5 = 9;
    int iran5 = 6;

    //# of goals conceded in last 5 games
    int italyC5 = 2;
    int portugalC5 = 4;
    int australiaC5 = 4;
    int iranC5 = 3;

    //# of victories in last 5 games
    int italyV5 = 2;
    int portugalV5 = 3;
    int australiaV5 = 2;
    int iranV5 = 3;

    //# of defeats in last 5 games
    int italyD5 = 1;
    int portugalD5 = 0;
    int australiaD5 = 1;
    int iranD5 = 0;


    //group B (Croatia, Belgium, Denmark, Columbia)

    int croatia = 0, belgium = 0, denmark = 0, columbia = 0;

    //attack
    int croatiaattack = 87;
    int belgiumattack = 89;
    int denmarkattack = 83;
    int columbiaattack = 85;

    //midfield
    int croatiamidfield = 90;
    int belgiummidfield = 89;
    int denmarkmidfield = 83;
    int columbiamidfield = 86;

    //defense
    int croatiadeffence = 87;
    int belgiumdeffence = 88;
    int denmarkdeffence = 84;
    int columbiadeffence = 82;

    //factor of unexpectancy
    int fcroatia = rand() % 100;
    int fbelgium = rand() % 100;
    int fdenmark = rand() % 100;
    int fcolumbia = rand() % 100;

    //currency in Euros
    double croatiacost = 355000000;
    double belgiumcost = 756000000;
    double denmarkcost = 262000000;
    double columbiacost = 256000000;
    
    //popuplation
    double croatiapop = 4153818;
    double belgiumpop = 11527032;
    double denmarkpop = 5763620;
    double columbiapop = 49635457;

    //# of goals score in last 5 games
    int croatia5 = 6;
    int belgium5 = 10;
    int denmark5 = 6;
    int columbia5 = 10;

    //# of goals conceded in last 5 games
    int croatiaC5 = 11;
    int belgiumC5 = 7;
    int denmarkC5 = 1;
    int columbiaC5 = 5;

    //# of victories in last 5 games
    int croatiaV5 = 2;
    int belgiumV5 = 3;
    int denmarkV5 = 3;
    int columbiaV5 = 3;

    //# of defeats in last 5 games
    int croatiaD5 = 2;
    int belgiumD5 = 1;
    int denmarkD5 = 0;
    int columbiaD5 = 1;

    //group C (Chile, Sweden, Netherlands, Mexico)

    int chile = 0, sweden = 0, netherlands = 0, mexico = 0;

    //attack
    int chileattack = 85;
    int swedenattack = 84;
    int netherlandsattack = 92;
    int mexicoattack = 87;

    //midfield
    int chilemidfield = 80;
    int swedenmidfield = 85;
    int netherlandsmidfield = 86;
    int mexicomidfield = 84;

    //defense
    int chiledeffence = 75;
    int swedendeffence = 80;
    int netherlandsdeffence = 85;
    int mexicodeffence = 80;

    //factor of unexpectancy
    int fchile = rand() % 100;
    int fsweden = rand() % 100;
    int fnetherlands = rand() % 100;
    int fmexico = rand() % 100;


    //currency in euros
    double chilecost = 125850000;
    double swedencost = 24000000;
    double netherlandscost = 511500000;
    double mexicocost = 97900000;

    //population
    double chilepop = 18259411;
    double swedenpop = 10014129;
    double netherlandspop = 17106100;
    double mexicopop = 131458115;

    //# of goals scored in last 5 games
    int chile5 = 7;
    int sweden5 = 6;
    int netherlands5 = 9;
    int mexico5 = 3;

    //# of goals condeded in the last 5 games
    int chileC5 = 7;
    int swedenC5 = 4;
    int netherlandsC5 = 5;
    int mexicoC5 = 8;

    //# of victories in the last 5 games
    int chileV5 = 2;
    int swedenV5 = 2;
    int netherlandsV5 = 2;
    int mexicoV5 = 1; 

    //# of defeats in the last 5 games
    int chileD5 = 2;
    int swedenD5 = 1;
    int netherlandsD5 = 1;
    int mexicoD5 = 4;

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

//factor of unexpectancy
    int fwales = rand() % 100;
    int fpoland = rand() % 100;
    int fusa = rand() % 100;
    int fperu = rand() % 100;

//cost
    double walescost = 228200000;
    double polandcost = 245400000;
    double usacost = 90150000;
    double perucost = 36980000;

    //population
    double walespop = 3188203;
    double polandpop = 38070590;
    double usapop = 327804709;
    double perupop = 32722047;

    //# of goals scored in last 5 games
    int wales5 = 3;
    int poland5 = 4;
    int usa5 = 4;
    int peru5 = 7;

    //# of goals conceded in the last 5 games
    int walesC5 = 9;
    int polandC5 = 7;
    int usaC5 = 9;
    int peruC5 = 9;

    //# of victories in the last 5 games
    int walesV5 = 1;
    int polandV5 = 0;
    int usaV5 = 1;
    int peruV5 = 1;

    //# of defeats in the last 5 games
    int walesD5 = 4;
    int polandD5 = 3;
    int usaD5 = 3;
    int peruD5 = 3;
     
 
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

 //factor of unexpectancy
    int fbrazil = rand() % 100;
    int fgermany = rand() % 100;
    int fsenegal = rand() % 100;
    int faustria = rand() % 100;

 //cost
     double brazilcost = 975000000;
     double germanycost = 922000000;
     double senegalcost = 237350000;
     double austriacost = 206500000;

     //population
     double brazilpop = 211548264;
     double germanypop = 82358331;
     double senegalpop = 16493754;
     double austriapop = 8758246;

     //# of goals scored in the last 5 games
     int brazil5 = 10;
     int germany5 = 8;
     int senegal5 = 7;
     int austria5 = 3;

     //# of goals conceded in the last 5 games
     int brazilC5 = 0;
     int germanyC5 = 8;
     int senegalC5 = 3;
     int austriaC5 = 4;

     //# of victories in the last 5 games
     int brazilV5 = 5;
     int germanyV5 = 2;
     int senegalV5 = 3;
     int austriaV5 = 2;

     //# of defeats in the last 5 games
     int brazilD5 = 0;
     int germanyD5 = 2;
     int senegalD5 = 1;
     int austriaD5 = 2;

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

 //factor of unexpectancy
    int fromania = rand() % 100;
    int ficeland = rand() % 100;
    int fengland = rand() % 100;
    int fspain = rand() % 100;

 //cost
     double romaniacost = 61950000;
     double icelandcost = 39380000;
     double englandcost = 979000000;
     double spaincost = 107000000;

     //population
     double romaniapop = 19537084;
     double icelandpop = 339023;
     double englandpop = 53012456;
     double spainpop = 46416939;

     //# of goals scored in the last 5 games
     int romania5 = 8;
     int iceland5 = 5;
     int england5 = 9;
     int spain5 = 15;

     //# of goals conceded in the last 5 games
     int romaniaC5 = 3;
     int icelandC5 = 11;
     int englandC5 = 3;
     int spainC5 = 7;

     //# of victories in the last 5 games
     int romaniaV5 = 3;
     int icelandV5 = 0;
     int englandV5 = 4;
     int spainV5 = 3;

     //# of defeats in the last 5 games
     int romaniaD5 = 0;
     int icelandD5 = 3;
     int englandD5 = 0;
     int spainD5 = 2;


 //group G (Argentina, France, Turkey, Russia) 

 int argentina = 0, france = 0, turkey = 0, russia = 0;

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

 //factor of unexpectancy
    int fargentina = rand() % 100;
    int ffrance = rand() % 100;
    int fturkey = rand() % 100;
    int frussia = rand() % 100;

 //cost
     double argentinacost = 566500000;
     double francecost = 103000000;
     double turkeycost = 132000000;
     double russiacost = 11100000;

     //population
     double argentinapop = 44873015;
     double francepop = 65343789;
     double turkeypop = 82382440;
     double russiapop = 143933783;

     //# of goals in the last 5 games
     int argentina5 = 8;
     int france5 = 7;
     int turkey5 = 3;
     int russia5 = 7;

     //# of goals condeded in the last 5 games
     int argentinaC5 = 1;
     int franceC5 = 6;
     int turkeyC5 = 4;
     int russiaC5 = 6;

     //# of victories in the last 5 games
     int argentinaV5 = 3;
     int franceV5 = 3;
     int turkeyV5 = 1;
     int russiaV5 = 2;

     //# of defeats in the last 5 games
     int argentinaD5 = 1;
     int franceD5 = 1;
     int turkeyD5 = 2;
     int russiaD5 = 2; 

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

 //factor of unexpectancy
    int furuguay = rand() % 100;
    int fserbia = rand() % 100;
    int fvenezuela = rand() % 100;
    int fmorocco = rand() % 100;

 //cost
     double uruguaycost = 32215000;
     double serbiacost = 249250000;
     double venezuelacost = 43700000;
     double moroccocost = 164450000;

     //population
     double uruguaypop = 3475182;
     double serbiapop = 8749218;
     double venezuelapop = 8749218;
     double moroccopop = 36389378;

     //# of goals scored in the last 5 games
     int uruguay5 = 7;
     int serbia5 = 10;
     int venezuela5 = 7;
     int morocco5 = 8;

     //# of goals conceded in the last 5 games
     int uruguayC5 = 9;
     int serbiaC5 = 4;
     int venezuelaC5 = 4; 
     int moroccoC5 = 2;

     //# of victories in the last 5 games
     int uruguayV5 = 1;
     int serbiaV5 = 3;
     int venezuelaV5 = 2;
     int moroccoV5 = 4;

     //# of defeats in the last 5 games
     int uruguayD5 = 4;
     int serbiaD5 = 0;
     int venezuelaD5 = 1; 
     int moroccoD5 = 0;

/////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

//Starting from backwards, i.e, starting from group H till group A, we have defined a bunch of if statements so that the coompiler can decide the result efficiently
//There are many if statements for this because every team's individual statistic is competing with every team's individual statistic.

 //group H


 //attack of uruguay
 if (uruguayattack > serbiaattack) {
     uruguay += 5;
 }
 if (uruguayattack > venezuelaattack) {
     uruguay += 5;
 }
 if (uruguayattack > moroccoattack) {
     uruguay += 5;
 }

 //attack of serbia
 if (serbiaattack > uruguayattack) {
     serbia += 5;
 }
 if (serbiaattack > venezuelaattack) {
     serbia += 5;
 }
 if (serbiaattack > moroccoattack) {
     serbia += 5;
 }

 //attack of venezuela
 if (venezuelaattack > uruguayattack) {
     venezuela += 5;
 } 
 if (venezuelaattack > serbiaattack) {
     venezuela += 5;
 }
 if (venezuelaattack > moroccoattack) {
     venezuela += 5;
 }

 //attack of morocco
 if (moroccoattack > uruguayattack) {
     morocco += 5;
 }
 if (moroccoattack > serbiaattack) {
     morocco += 5;
 }
 if (moroccoattack > venezuelaattack) {
     morocco += 5;
 }

 //midfield of uruguay
 if (uruguaymidfield > serbiamidfield) {
     uruguay += 5;
 }
 if (uruguaymidfield > venezuelamidfield) {
     uruguay += 5;
 }
 if (uruguaymidfield > moroccomidfield) {
     uruguay += 5;
 }

 //midfield of serbia
 if (serbiamidfield > uruguaymidfield ) {
     serbia += 5;
 }
 if (serbiamidfield > venezuelamidfield ) {
     serbia += 5;
 }
 if (serbiamidfield > moroccomidfield ) {
     serbia += 5;
 }

 //midfield of venezuela
 if (venezuelamidfield > uruguaymidfield) {
     venezuela += 5;
 }
 if (venezuelamidfield > serbiamidfield) {
     venezuela += 5;
 }
 if (venezuelamidfield > moroccomidfield) {
     venezuela += 5;
 }

 //midfield of morocco
 if (moroccomidfield > uruguaymidfield) {
     morocco += 5;
 }
 if (moroccomidfield > serbiamidfield) {
     morocco += 5;
 }
 if (moroccomidfield > venezuelamidfield) {
     morocco += 5;
 }

 //defense of uruguay
 if (uruguaydeffence > serbiadeffence) {
     uruguay += 5;
 }
 if (uruguaydeffence > venezueladeffence) {
     uruguay += 5;
 }
 if (uruguaydeffence > moroccodeffence) {
     uruguay += 5;
 }

 //defense of venezuela
 if (venezueladeffence > serbiadeffence) {
     venezuela += 5;
 }
 if (venezueladeffence > uruguaydeffence) {
     venezuela += 5;
 }
 if (venezueladeffence > moroccodeffence) {
     venezuela += 5;
 }

 //defense of serbia
 if (serbiadeffence > uruguaydeffence) {
     serbia += 5;
 }
 if (serbiadeffence > venezueladeffence) {
     serbia += 5;
 }
 if (serbiadeffence > moroccodeffence) {
     serbia += 5;
 }

 //defense of morocco
 if (moroccodeffence > uruguaydeffence) {
     morocco += 5;
 }
 if (moroccodeffence > serbiadeffence) {
     morocco += 5;
 }
 if (moroccodeffence > venezueladeffence) {
     morocco += 5;
 }


    //cost of morocco
    if (moroccocost > uruguaycost) {
        morocco += 3;
    }
    
    if (moroccocost > serbiacost) {
        morocco += 3;
    }

    if (moroccocost > venezuelacost) {
        morocco += 3;
    }

    //cost of uruguay
    if (uruguaycost > moroccocost) {
        uruguay += 3;
    }
    
    if (uruguaycost > serbiacost) {
        uruguay += 3;
    }

    if (uruguaycost > venezuelacost) {
        uruguay += 3;
    }

    //cost of serbia
    if (serbiacost > moroccocost) {
        serbia += 3;
    }
    
    if (serbiacost > uruguaycost) {
        serbia += 3;
    }

    if (serbiacost > venezuelacost) {
        serbia += 3;
    }

    //cost of venezuela
    if (venezuelacost > moroccocost) {
        venezuela += 3;
    }
    
    if (venezuelacost > uruguaycost) {
        venezuela += 3;
    }

    if (venezuelacost > serbiacost) {
        venezuela += 3;
    }

    //population of morocco
    if (moroccopop > venezuelapop) {
        morocco += 3;
    }
    
    if (moroccopop > uruguaypop) {
        morocco += 3;
    }

    if (moroccopop > serbiapop) {
        morocco += 3;
    }

    //population of venezuela
    if (venezuelapop > moroccopop) {
        venezuela += 3;
    }
    
    if (venezuelapop > uruguaypop) {
        venezuela += 3;
    }

    if (venezuelapop > serbiapop) {
        venezuela += 3;
    }

    //population of uruguay
    if (uruguaypop > moroccopop) {
        uruguay += 3;
    }
    
    if (uruguaypop > venezuelapop) {
        uruguay += 3;
    }

    if (uruguaypop > serbiapop) {
        uruguay += 3;
    }

    //population of serbia
    if (serbiapop > moroccopop) {
        serbia += 3;
    }
    
    if (serbiapop > venezuelapop) {
        serbia += 3;
    }

    if (serbiapop > uruguaypop) {
        serbia += 3;
    }

    

    //morocco # of goals score in last 5 games
    if (morocco5 > serbia5) {
        morocco += 1;
    }
    
    if (morocco5 > venezuela5) {
        morocco += 1;
    }

    if (morocco5 > uruguay5) {
        morocco += 1;
    }

    //serbia # of goals score in last 5 games
    if (serbia5 > morocco5) {
        serbia += 1;
    }
    
    if (serbia5 > venezuela5) {
        serbia += 1;
    }

    if (serbia5 > uruguay5) {
        serbia += 1;
    }

    //venezuela # of goals score in last 5 games
    if (venezuela5 > morocco5) {
        venezuela += 1;
    }
    
    if (venezuela5 > serbia5) {
        venezuela += 1;
    }

    if (venezuela5 > uruguay5) {
        venezuela += 1;
    }
    
    //uruguay # of goals score in last 5 games
    if (uruguay5 > morocco5) {
        uruguay += 1;
    }
    
    if (uruguay5 > serbia5) {
        uruguay += 1;
    }

    if (uruguay5 > venezuela5) {
        uruguay += 1;
    }

    //morocco # of goals conceded in last 5 games
    if (moroccoC5 > uruguayC5) {
        morocco -= 1;
    }
    
    if (moroccoC5 > serbiaC5) {
        morocco -= 1;
    }

    if (moroccoC5 > venezuelaC5) {
        morocco -= 1;
    }
    
    //uruguay # of goals conceded in last 5 games
    if (uruguayC5 > moroccoC5) {
        uruguay -= 1;
    }
    
    if (uruguayC5 > serbiaC5) {
        uruguay -= 1;
    }

    if (uruguayC5 > venezuelaC5) {
        uruguay -= 1;
    }

    //serbia # of goals conceded in last 5 games
    if (serbiaC5 > moroccoC5) {
        serbia -= 1;
    }
    
    if (serbiaC5 > uruguayC5) {
        serbia -= 1;
    }

    if (serbiaC5 > venezuelaC5) {
        serbia -= 1;
    }

    //venezuela # of goals conceded in last 5 games
    if (venezuelaC5 > moroccoC5) {
        venezuela -= 1;
    }
    
    if (venezuelaC5 > uruguayC5) {
        venezuela -= 1;
    }

    if (venezuelaC5 > serbiaC5) {
        venezuela -= 1;
    }

    //morocco # of goals victory in last 5 games
    if (moroccoV5 > venezuelaV5) {
        morocco += 1;
    }
    
    if (moroccoV5 > uruguayV5) {
        morocco += 1;
    }

    if (moroccoV5 > serbiaV5) {
        morocco += 1;
    }

    //venezuela # of goals victory in last 5 games
    if (venezuelaV5 > moroccoV5) {
        venezuela += 1;
    }
    
    if (venezuelaV5 > uruguayV5) {
        venezuela += 1;
    }

    if (venezuelaV5 > serbiaV5) {
        venezuela += 1;
    }

    //uruguay # of goals victory in last 5 games
    if (uruguayV5 > moroccoV5) {
        uruguay += 1;
    }
    
    if (uruguayV5 > venezuelaV5) {
        uruguay += 1;
    }

    if (uruguayV5 > serbiaV5) {
        uruguay += 1;
    }

    //serbia # of goals victory in last 5 games
    if (serbiaV5 > moroccoV5) {
        serbia += 1;
    }
    
    if (serbiaV5 > venezuelaV5) {
        serbia += 1;
    }

    if (serbiaV5 > uruguayV5) {
        serbia += 1;
    }

    //morocco # of defeats in last 5 games
    if (moroccoD5 > serbiaD5) {
        morocco -= 1;
    }
    
    if (moroccoD5 > venezuelaD5) {
        morocco -= 1;
    }

    if (moroccoD5 > uruguayD5) {
        morocco -= 1;
    }

    //serbia # of defeats in last 5 games
    if (serbiaD5 > moroccoD5) {
        serbia -= 1;
    }
    
    if (serbiaD5 > venezuelaD5) {
        serbia -= 1;
    }

    if (serbiaD5 > uruguayD5) {
        serbia -= 1;
    }

    //venezuela # of defeats in last 5 games
    if (venezuelaD5 > moroccoD5) {
        venezuela -= 1;
    }
    
    if (venezuelaD5 > serbiaD5) {
        venezuela -= 1;
    }

    if (venezuelaD5 > uruguayD5) {
        venezuela -= 1;
    }

    //uruguay # of defeats in last 5 games
    if (uruguayD5 > moroccoD5) {
        uruguay -= 1;
    }
    
    if (uruguayD5 > serbiaD5) {
        uruguay -= 1;
    }

    if (uruguayD5 > venezuelaD5) {
        uruguay -= 1;
    }

    //morocco factor of unexpectancy
    if (fmorocco > furuguay) {
        morocco = morocco + r1;
    }
    
    if (fmorocco > fserbia) {
        morocco = morocco + r1;
    }

    if (fmorocco > fvenezuela) {
        morocco = morocco + r1;
    }

    //uruguay factor of unexpectancy
    if (furuguay > fmorocco) {
        uruguay = uruguay + r2;
    }
    
    if (furuguay > fserbia) {
        uruguay = uruguay + r2;
    }

    if (furuguay > fvenezuela) {
        uruguay = uruguay + r2;
    }

    //serbia factor of unexpectancy
    if (fserbia > fmorocco) {
        serbia = serbia + r3;
    }
    
    if (fserbia > furuguay) {
        serbia = serbia + r3;
    }

    if (fserbia > fvenezuela) {
        serbia = serbia + r3;
    }

    //venezuela factor of unexpectancy
    if (fvenezuela > fmorocco) {
        venezuela = venezuela + r4;
    }
    
    if (fvenezuela > furuguay) {
        venezuela = venezuela + r4;
    }

    if (fvenezuela > fserbia) {
        venezuela = venezuela + r4;
    }
    
    //To be a winner for group H, a team has to have the most points among the other teams in this group and so we have made the following simulator that compares every team in a particular group against every team in the same group
 
 //1st place result of group H
if (uruguay > serbia && uruguay > morocco && uruguay > venezuela) {
    cout << "Uruguay is the winner of Group H" << endl;
    Q1groupH = uruguay;
    Q1groupHattack = uruguayattack;
    Q1groupHmidfield = uruguaymidfield;
    Q1groupHdeffence = uruguaydeffence;
    Q1groupHf = furuguay;
    Q1groupHcost = uruguaycost;
    Q1groupHpop = uruguaypop;
    Q1groupH5 = uruguay5;
    Q1groupHC5 = uruguayC5;
    Q1groupHV5 = uruguayV5;
    Q1groupHD5 = uruguayD5;
    FQ1groupH = "Uruguay";
}
else if (serbia > uruguay && serbia > morocco && serbia > venezuela) {
    cout << "Serbia is the winner of Group H" << endl;
    Q1groupH = serbia;
    Q1groupHattack = serbiaattack;
    Q1groupHmidfield = serbiamidfield;
    Q1groupHdeffence = serbiadeffence;
    Q1groupHf = fserbia;
    Q1groupHcost = serbiacost;
    Q1groupHpop = serbiapop;
    Q1groupH5 = serbia5;
    Q1groupHC5 = serbiaC5;
    Q1groupHV5 = serbiaV5;
    Q1groupHD5 = serbiaD5;
    FQ1groupH = "Serbia";
}
else if (morocco > uruguay && morocco > serbia && morocco > venezuela) {
    cout << "Morocco is the winner of Group H" << endl;
    Q1groupH = morocco;
    Q1groupHattack = moroccoattack;
    Q1groupHmidfield = moroccomidfield;
    Q1groupHdeffence = moroccodeffence;
    Q1groupHf = fmorocco;
    Q1groupHcost = moroccocost;
    Q1groupHpop = moroccopop;
    Q1groupH5 = morocco5;
    Q1groupHC5 = moroccoC5;
    Q1groupHV5 = moroccoV5;
    Q1groupHD5 = moroccoD5;
    FQ1groupH = "Morocco";
}
else if (venezuela > uruguay && venezuela > morocco && venezuela > serbia) {
    cout << "Venezuela is the winner of Group H" << endl;
    Q1groupH = venezuela;
    Q1groupHattack = venezuelaattack;
    Q1groupHmidfield = venezuelamidfield;
    Q1groupHdeffence = venezueladeffence;
    Q1groupHf = fvenezuela;
    Q1groupHcost = venezuelacost;
    Q1groupHpop = venezuelapop;
    Q1groupH5 = venezuela5;
    Q1groupHC5 = venezuelaC5;
    Q1groupHV5 = venezuelaV5;
    Q1groupHD5 = venezuelaD5;
    FQ1groupH = "Venezuela";
}

//Similarly, we have also designed a simulator that will show which team stands in the second position of a group.

   //2nd place results of group H 

    //uruguay
    if (uruguay > serbia && uruguay > morocco && uruguay < venezuela) {
    cout << "Uruguay is the second of Group H" << endl;
    Q2groupH = uruguay;
    Q2groupHattack = uruguayattack;
    Q2groupHmidfield = uruguaymidfield;
    Q2groupHdeffence = uruguaydeffence;
    Q2groupHf = furuguay;
    Q2groupHcost = uruguaycost;
    Q2groupHpop = uruguaypop;
    Q2groupH5 = uruguay5;
    Q2groupHC5 = uruguayC5;
    Q2groupHV5 = uruguayV5;
    Q2groupHD5 = uruguayD5;
    FQ2groupH = "Uruguay";
    
}

else if (uruguay > serbia && uruguay < morocco && uruguay > venezuela) {
    cout << "Uruguay is the second of Group H" << endl;
    Q2groupH = uruguay;
    Q2groupHattack = uruguayattack;
    Q2groupHmidfield = uruguaymidfield;
    Q2groupHdeffence = uruguaydeffence;
    FQ2groupH = "Uruguay";
    Q2groupHf = furuguay;
    Q2groupHcost = uruguaycost;
    Q2groupHpop = uruguaypop;
    Q2groupH5 = uruguay5;
    Q2groupHC5 = uruguayC5;
    Q2groupHV5 = uruguayV5;
    Q2groupHD5 = uruguayD5;
}

else if (uruguay < serbia && uruguay > morocco && uruguay > venezuela) {
    cout << "Uruguay is the second of Group H" << endl;
    Q2groupH = uruguay;
    Q2groupHattack = uruguayattack;
    Q2groupHmidfield = uruguaymidfield;
    Q2groupHdeffence = uruguaydeffence;
    FQ2groupH = "Uruguay";
    Q2groupHf = furuguay;
    Q2groupHcost = uruguaycost;
    Q2groupHpop = uruguaypop;
    Q2groupH5 = uruguay5;
    Q2groupHC5 = uruguayC5;
    Q2groupHV5 = uruguayV5;
    Q2groupHD5 = uruguayD5;
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
    Q2groupHf = fserbia;
    Q2groupHcost = serbiacost;
    Q2groupHpop = serbiapop;
    Q2groupH5 = serbia5;
    Q2groupHC5 = serbiaC5;
    Q2groupHV5 = serbiaV5;
    Q2groupHD5 = serbiaD5;
}
else if (serbia > uruguay && serbia < morocco && serbia > venezuela) {
    cout << "Serbia is the second of Group H" << endl;
    Q2groupH = serbia;
    Q2groupHattack = serbiaattack;
    Q2groupHmidfield = serbiamidfield;
    Q2groupHdeffence = serbiadeffence;
    FQ2groupH = "Serbia";
    Q2groupHf = fserbia;
    Q2groupHcost = serbiacost;
    Q2groupHpop = serbiapop;
    Q2groupH5 = serbia5;
    Q2groupHC5 = serbiaC5;
    Q2groupHV5 = serbiaV5;
    Q2groupHD5 = serbiaD5;
}
else if (serbia < uruguay && serbia > morocco && serbia > venezuela) {
    cout << "Serbia is the second of Group H" << endl;
    Q2groupH = serbia;
    Q2groupHattack = serbiaattack;
    Q2groupHmidfield = serbiamidfield;
    Q2groupHdeffence = serbiadeffence;
    FQ2groupH = "Serbia";
    Q2groupHf = fserbia;
    Q2groupHcost = serbiacost;
    Q2groupHpop = serbiapop;
    Q2groupH5 = serbia5;
    Q2groupHC5 = serbiaC5;
    Q2groupHV5 = serbiaV5;
    Q2groupHD5 = serbiaD5;
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
    Q2groupHf = fvenezuela;
    Q2groupHcost = venezuelacost;
    Q2groupHpop = venezuelapop;
    Q2groupH5 = venezuela5;
    Q2groupHC5 = venezuelaC5;
    Q2groupHV5 = venezuelaV5;
    Q2groupHD5 = venezuelaD5;
    
}
else if (venezuela > uruguay && venezuela < morocco && venezuela > serbia) {
    cout << "Venezuela is the second of Group H" << endl;
    Q2groupH = venezuela;
    Q2groupHattack = venezuelaattack;
    Q2groupHmidfield = venezuelamidfield;
    Q2groupHdeffence = venezueladeffence;
    FQ2groupH = "Venezuela";
    Q2groupHf = fvenezuela;
    Q2groupHcost = venezuelacost;
    Q2groupHpop = venezuelapop;
    Q2groupH5 = venezuela5;
    Q2groupHC5 = venezuelaC5;
    Q2groupHV5 = venezuelaV5;
    Q2groupHD5 = venezuelaD5;
}
else if (venezuela < uruguay && venezuela > morocco && venezuela > serbia) {
    cout << "Venezuela is the second of Group H" << endl;
    Q2groupH = venezuela;
    Q2groupHattack = venezuelaattack;
    Q2groupHmidfield = venezuelamidfield;
    Q2groupHdeffence = venezueladeffence;
    FQ2groupH = "Venezuela";
    Q2groupHf = fvenezuela;
    Q2groupHcost = venezuelacost;
    Q2groupHpop = venezuelapop;
    Q2groupH5 = venezuela5;
    Q2groupHC5 = venezuelaC5;
    Q2groupHV5 = venezuelaV5;
    Q2groupHD5 = venezuelaD5;
}
else {}

//morocco
if (morocco > uruguay && morocco > venezuela && morocco < serbia) {
    cout << "Morocco is the second of Group H" << endl;
    Q2groupH = morocco;
    Q2groupHattack = moroccoattack;
    Q2groupHmidfield = moroccomidfield;
    Q2groupHdeffence = moroccodeffence;
    FQ2groupH = "Morocco";
    Q2groupHf = fmorocco;
    Q2groupHcost = moroccocost;
    Q2groupHpop = moroccopop;
    Q2groupH5 = morocco5;
    Q2groupHC5 = moroccoC5;
    Q2groupHV5 = moroccoV5;
    Q2groupHD5 = moroccoD5;
}
else if (morocco > uruguay && morocco < venezuela && morocco > serbia) {
    cout << "Morocco is the second of Group H" << endl;
    Q2groupH = morocco;
    Q2groupHattack = moroccoattack;
    Q2groupHmidfield = moroccomidfield;
    Q2groupHdeffence = moroccodeffence;
    FQ2groupH = "Morocco";
    Q2groupHf = fmorocco;
    Q2groupHcost = moroccocost;
    Q2groupHpop = moroccopop;
    Q2groupH5 = morocco5;
    Q2groupHC5 = moroccoC5;
    Q2groupHV5 = moroccoV5;
    Q2groupHD5 = moroccoD5;
}
else if (morocco < uruguay && morocco > venezuela && morocco > serbia) {
    cout << "Morocco is the second of Group H" << endl;
    Q2groupH = morocco;
    Q2groupHattack = moroccoattack;
    Q2groupHmidfield = moroccomidfield;
    Q2groupHdeffence = moroccodeffence;
    FQ2groupH = "Morocco";
    Q2groupHf = fmorocco;
    Q2groupHcost = moroccocost;
    Q2groupHpop = moroccopop;
    Q2groupH5 = morocco5;
    Q2groupHC5 = moroccoC5;
    Q2groupHV5 = moroccoV5;
    Q2groupHD5 = moroccoD5;
}
else {}


    //There are many if statements for this because every team's individual statistic is competing with every team's individual statistic.

    //group G


    //attack of argentina
 if (argentinaattack > franceattack) {
     argentina += 5;
 }
 if (argentinaattack > turkeyattack) {
     argentina += 5;
 }
 if (argentinaattack > russiaattack) {
     argentina += 5;
 }

 //attack of france
 if (franceattack > argentinaattack) { 
     franceattack += 5;
 }
 if (franceattack > turkeyattack) { 
     franceattack += 5;
 }
 if (franceattack > russiaattack) { 
     franceattack += 5;
 }

 //attack of turkey
 if (turkeyattack > argentinaattack) {
     turkey += 5;
 }
 if (turkeyattack > franceattack) {
     turkey += 5;
 }
 if (turkeyattack > russiaattack) {
     turkey += 5;
 }

 //attack of russia
 if (russiaattack > argentinaattack) {
     russia += 5;
 }
 if (russiaattack > franceattack) {
     russia += 5;
 }
 if (russiaattack > turkeyattack) {
     russia += 5;
 }

 //midfield of argentina 
if (argentinamidfield > francemidfield) {
     argentina += 5;
 }
 if (argentinamidfield > turkeymidfield) {
     argentina += 5;
 }
 if (argentinamidfield > russiamidfield) {
     argentina += 5;
 }

 //midfield of france
 if (francemidfield > argentinamidfield) {
     france += 5;
 }
 if (francemidfield > turkeymidfield) {
     france += 5;
 }
 if (francemidfield > russiamidfield) {
     france += 5;
 }

 //midfield of turkey
 if (turkeymidfield > argentinamidfield) {
     turkey += 5;
 }
 if (turkeymidfield > francemidfield) {
     turkey += 5;
 }
 if (turkeymidfield > russiamidfield) {
     turkey += 5;
 }

 //midfield of russia
 if (russiamidfield > argentinamidfield) {
     russia += 5;
 }
 if (russiamidfield > francemidfield) {
     russia += 5;
 }
 if (russiamidfield > turkeymidfield) {
     russia += 5;
 }

 //defense of argentina
 if (argentinadeffence > francedeffence) {
     argentina += 5;
 }
 if (argentinadeffence > turkeydeffence) {
     argentina += 5;
 }
 if (argentinadeffence > russiadeffence) {
     argentina += 5;
 }

 //defense of france
 if (francedeffence > argentinadeffence) {
     france += 5;
 }
 if (francedeffence > turkeydeffence) {
     france += 5;
 }
 if (francedeffence > russiadeffence) {
     france += 5;
 }

 //defense of turkey
 if (turkeydeffence > argentinadeffence) {
     turkey += 5;
 }
 if (turkeydeffence > francedeffence) {
     turkey += 5;
 }
 if (turkeydeffence > russiadeffence) {
     turkey += 5;
 }

 //defense of russia
 if (russiadeffence > argentinadeffence) {
     russia += 5;
 }
 if (russiadeffence > francedeffence) {
     russia += 5;
 }
 if (russiadeffence > turkeydeffence) {
     russia += 5;
 }

 //cost of russia
    if (russiacost > argentinacost) {
        russia += 3;
    }
    
    if (russiacost > francecost) {
        russia += 3;
    }

    if (russiacost > turkeycost) {
        russia += 3;
    }

    //cost of argentina
    if (argentinacost > russiacost) {
        argentina += 3;
    }
    
    if (argentinacost > francecost) {
        argentina += 3;
    }

    if (argentinacost > turkeycost) {
        argentina += 3;
    }

    //cost of france
    if (francecost > russiacost) {
        france += 3;
    }
    
    if (francecost > argentinacost) {
        france += 3;
    }

    if (francecost > turkeycost) {
        france += 3;
    }

    //cost of turkey
    if (turkeycost > russiacost) {
        turkey += 3;
    }
    
    if (turkeycost > argentinacost) {
        turkey += 3;
    }

    if (turkeycost > francecost) {
        turkey += 3;
    }

    //population of russia
    if (russiapop > turkeypop) {
        russia += 3;
    }
    
    if (russiapop > argentinapop) {
        russia += 3;
    }

    if (russiapop > francepop) {
        russia += 3;
    }

    //population of turkey
    if (turkeypop > russiapop) {
        turkey += 3;
    }
    
    if (turkeypop > argentinapop) {
        turkey += 3;
    }

    if (turkeypop > francepop) {
        turkey += 3;
    }

    //population of argentina
    if (argentinapop > russiapop) {
        argentina += 3;
    }
    
    if (argentinapop > turkeypop) {
        argentina += 3;
    }

    if (argentinapop > francepop) {
        argentina += 3;
    }

    //population of france
    if (francepop > russiapop) {
        france += 3;
    }
    
    if (francepop > turkeypop) {
        france += 3;
    }

    if (francepop > argentinapop) {
        france += 3;
    }

    //russia # of goals score in last 5 games
    if (russia5 > france5) {
        russia += 1;
    }
    
    if (russia5 > turkey5) {
        russia += 1;
    }

    if (russia5 > argentina5) {
        russia += 1;
    }

    //france # of goals score in last 5 games
    if (france5 > russia5) {
        france += 1;
    }
    
    if (france5 > turkey5) {
        france += 1;
    }

    if (france5 > argentina5) {
        france += 1;
    }

    //turkey # of goals score in last 5 games
    if (turkey5 > russia5) {
        turkey += 1;
    }
    
    if (turkey5 > france5) {
        turkey += 1;
    }

    if (turkey5 > argentina5) {
        turkey += 1;
    }
    
    //argentina # of goals score in last 5 games
    if (argentina5 > russia5) {
        argentina += 1;
    }
    
    if (argentina5 > france5) {
        argentina += 1;
    }

    if (argentina5 > turkey5) {
        argentina += 1;
    }

    //russia # of goals conceded in last 5 games
    if (russiaC5 > argentinaC5) {
        russia -= 1;
    }
    
    if (russiaC5 > franceC5) {
        russia -= 1;
    }

    if (russiaC5 > turkeyC5) {
        russia -= 1;
    }
    
    //argentina # of goals conceded in last 5 games
    if (argentinaC5 > russiaC5) {
        argentina -= 1;
    }
    
    if (argentinaC5 > franceC5) {
        argentina -= 1;
    }

    if (argentinaC5 > turkeyC5) {
        argentina -= 1;
    }

    //france # of goals conceded in last 5 games
    if (franceC5 > russiaC5) {
        france -= 1;
    }
    
    if (franceC5 > argentinaC5) {
        france -= 1;
    }

    if (franceC5 > turkeyC5) {
        france -= 1;
    }

    //turkey # of goals conceded in last 5 games
    if (turkeyC5 > russiaC5) {
        turkey -= 1;
    }
    
    if (turkeyC5 > argentinaC5) {
        turkey -= 1;
    }

    if (turkeyC5 > franceC5) {
        turkey -= 1;
    }

    //russia # of goals victory in last 5 games
    if (russiaV5 > turkeyV5) {
        russia += 1;
    }
    
    if (russiaV5 > argentinaV5) {
        russia += 1;
    }

    if (russiaV5 > franceV5) {
        russia += 1;
    }

    //turkey # of goals victory in last 5 games
    if (turkeyV5 > russiaV5) {
        turkey += 1;
    }
    
    if (turkeyV5 > argentinaV5) {
        turkey += 1;
    }

    if (turkeyV5 > franceV5) {
        turkey += 1;
    }

    //argentina # of goals victory in last 5 games
    if (argentinaV5 > russiaV5) {
        argentina += 1;
    }
    
    if (argentinaV5 > turkeyV5) {
        argentina += 1;
    }

    if (argentinaV5 > franceV5) {
        argentina += 1;
    }

    //france # of goals victory in last 5 games
    if (franceV5 > russiaV5) {
        france += 1;
    }
    
    if (franceV5 > turkeyV5) {
        france += 1;
    }

    if (franceV5 > argentinaV5) {
        france += 1;
    }

    //russia # of defeats in last 5 games
    if (russiaD5 > franceD5) {
        russia -= 1;
    }
    
    if (russiaD5 > turkeyD5) {
        russia -= 1;
    }

    if (russiaD5 > argentinaD5) {
        russia -= 1;
    }

    //france # of defeats in last 5 games
    if (franceD5 > russiaD5) {
        france -= 1;
    }
    
    if (franceD5 > turkeyD5) {
        france -= 1;
    }

    if (franceD5 > argentinaD5) {
        france -= 1;
    }

    //turkey # of defeats in last 5 games
    if (turkeyD5 > russiaD5) {
        turkey -= 1;
    }
    
    if (turkeyD5 > franceD5) {
        turkey -= 1;
    }

    if (turkeyD5 > argentinaD5) {
        turkey -= 1;
    }

    //argentina # of defeats in last 5 games
    if (argentinaD5 > russiaD5) {
        argentina -= 1;
    }
    
    if (argentinaD5 > franceD5) {
        argentina -= 1;
    }

    if (argentinaD5 > turkeyD5) {
        argentina -= 1;
    }

    //russia factor of unexpectancy
    if (frussia > fargentina) {
        russia = russia + r5;
    }
    
    if (frussia > ffrance) {
        russia = russia + r5;
    }

    if (frussia > fturkey) {
        russia = russia + r5;
    }

    //argentina factor of unexpectancy
    if (fargentina > frussia) {
        argentina = argentina + r6;
    }
    
    if (fargentina > ffrance) {
        argentina = argentina + r6;
    }

    if (fargentina > fturkey) {
        argentina = argentina + r6;
    }

    //france factor of unexpectancy
    if (ffrance > frussia) {
        france = france + r7;
    }
    
    if (ffrance > fargentina) {
        france = france + r7;
    }

    if (ffrance > fturkey) {
        france = france + r7;
    }

    //turkey factor of unexpectancy
    if (fturkey > frussia) {
        turkey = turkey + r8;
    }
    
    if (fturkey > fargentina) {
        turkey = turkey + r8;
    }

    if (fturkey > ffrance) {
        turkey = turkey + r8;
    }



 //1st place results of group G
 if (argentina > russia && argentina > france && argentina > turkey) {
    cout << "Argentina is the winner of Group G" << endl;
    Q1groupG = argentina;
    Q1groupGattack = argentinaattack;
    Q1groupGmidfield = argentinamidfield;
    Q1groupGdeffence = argentinadeffence;
    FQ1groupG = "Argentina";
    Q1groupGf = fargentina;
    Q1groupGcost = argentinacost;
    Q1groupGpop = argentinapop;
    Q1groupG5 = argentina5;
    Q1groupGC5 = argentinaC5;
    Q1groupGV5 = argentinaV5;
    Q1groupGD5 = argentinaD5;
}
else if (russia > argentina && russia > france && russia > turkey) {
    cout << "Russia is the winner of Group G" << endl;
    Q1groupG = russia;
    Q1groupGattack = russiaattack;
    Q1groupGmidfield = russiamidfield;
    Q1groupGdeffence = russiadeffence;
    FQ1groupG = "Russia";
    Q1groupGf = frussia;
    Q1groupGcost = russiacost;
    Q1groupGpop = russiapop;
    Q1groupG5 = russia5;
    Q1groupGC5 = russiaC5;
    Q1groupGV5 = russiaV5;
    Q1groupGD5 = russiaD5;
}
else if (france > argentina && france > russia && france > turkey) {
    cout << "France is the winner of Group G" << endl;
    Q1groupG = france;
    Q1groupGattack = franceattack;
    Q1groupGmidfield = francemidfield;
    Q1groupGdeffence = francedeffence;
    FQ1groupG = "France";
    Q1groupGf = ffrance;
    Q1groupGcost = francecost;
    Q1groupGpop = francepop;
    Q1groupG5 = france5;
    Q1groupGC5 = franceC5;
    Q1groupGV5 = franceV5;
    Q1groupGD5 = franceD5;
}
else if (turkey > argentina && turkey > france && turkey > russia) {
    cout << "Turkey is the winner of Group G" << endl;
    Q1groupG = turkey;
    Q1groupGattack = turkeyattack;
    Q1groupGmidfield = turkeymidfield;
    Q1groupGdeffence = turkeydeffence;
    FQ1groupG = "Turkey";
    Q1groupGf = fturkey;
    Q1groupGcost = turkeycost;
    Q1groupGpop = turkeypop;
    Q1groupG5 = turkey5;
    Q1groupGC5 = turkeyC5;
    Q1groupGV5 = turkeyV5;
    Q1groupGD5 = turkeyD5;
}

//2nd place result of group G

//argentina
if (argentina > france && argentina > russia && argentina < turkey) {
    cout << "Argentina is the second of Group G" << endl;
    Q2groupG = argentina;
    Q2groupGattack = argentinaattack;
    Q2groupGmidfield = argentinamidfield;
    Q2groupGdeffence = argentinadeffence;
    FQ2groupG = "Argentina";
    Q2groupGf = fargentina;
    Q2groupGcost = argentinacost;
    Q2groupGpop = argentinapop;
    Q2groupG5 = argentina5;
    Q2groupGC5 = argentinaC5;
    Q2groupGV5 = argentinaV5;
    Q2groupGD5 = argentinaD5;
}
else if (argentina > france && argentina < russia && argentina > turkey) {
    cout << "Argentina is the second of Group G" << endl;
    Q2groupG = argentina;
    Q2groupGattack = argentinaattack;
    Q2groupGmidfield = argentinamidfield;
    Q2groupGdeffence = argentinadeffence;
    FQ2groupG = "Argentina";
    Q2groupGf = fargentina;
    Q2groupGcost = argentinacost;
    Q2groupGpop = argentinapop;
    Q2groupG5 = argentina5;
    Q2groupGC5 = argentinaC5;
    Q2groupGV5 = argentinaV5;
    Q2groupGD5 = argentinaD5;
}
else if (argentina < france && argentina > russia && argentina > turkey) {
    cout << "Argentina is the second of Group G" << endl;
    Q2groupG = argentina;
    Q2groupGattack = argentinaattack;
    Q2groupGmidfield = argentinamidfield;
    Q2groupGdeffence = argentinadeffence;
    FQ2groupG = "Argentina";
    Q2groupGf = fargentina;
    Q2groupGcost = argentinacost;
    Q2groupGpop = argentinapop;
    Q2groupG5 = argentina5;
    Q2groupGC5 = argentinaC5;
    Q2groupGV5 = argentinaV5;
    Q2groupGD5 = argentinaD5;
}
else {}


//france
if (france > argentina && france > russia && france < turkey) {
    cout << "France is the second of Group G" << endl;
    Q2groupG = france;
    Q2groupGattack = franceattack;
    Q2groupGmidfield = francemidfield;
    Q2groupGdeffence = francedeffence;
    FQ2groupG = "France";
    Q2groupGf = ffrance;
    Q2groupGcost = francecost;
    Q2groupGpop = francepop;
    Q2groupG5 = france5;
    Q2groupGC5 = franceC5;
    Q2groupGV5 = franceV5;
    Q2groupGD5 = franceD5;
}
else if (france > argentina && france < russia && france > turkey) {
    cout << "France is the second of Group G" << endl;
    Q2groupG = france;
    Q2groupGattack = franceattack;
    Q2groupGmidfield = francemidfield;
    Q2groupGdeffence = francedeffence;
    FQ2groupG = "France";
    Q2groupGf = ffrance;
    Q2groupGcost = francecost;
    Q2groupGpop = francepop;
    Q2groupG5 = france5;
    Q2groupGC5 = franceC5;
    Q2groupGV5 = franceV5;
    Q2groupGD5 = franceD5;
}
else if (france < argentina && france > russia && france > turkey) {
    cout << "France is the second of Group G" << endl;
    Q2groupG = france;
    Q2groupGattack = franceattack;
    Q2groupGmidfield = francemidfield;
    Q2groupGdeffence = francedeffence;
    FQ2groupG = "France";
    Q2groupGf = ffrance;
    Q2groupGcost = francecost;
    Q2groupGpop = francepop;
    Q2groupG5 = france5;
    Q2groupGC5 = franceC5;
    Q2groupGV5 = franceV5;
    Q2groupGD5 = franceD5;
}
else {}

//russia
if (russia > argentina && russia > france && russia < turkey) {
    cout << "Russia is the second of Group G" << endl;
    Q2groupG = russia;
    Q2groupGattack = russiaattack;
    Q2groupGmidfield = russiamidfield;
    Q2groupGdeffence = russiadeffence;
    FQ2groupG = "Russia";
    Q2groupGf = frussia;
    Q2groupGcost = russiacost;
    Q2groupGpop = russiapop;
    Q2groupG5 = russia5;
    Q2groupGC5 = russiaC5;
    Q2groupGV5 = russiaV5;
    Q2groupGD5 = russiaD5;
}
else if (russia > argentina && russia < france && russia > turkey) {
    cout << "Russia is the second of Group G" << endl;
    Q2groupG = russia;
    Q2groupGattack = russiaattack;
    Q2groupGmidfield = russiamidfield;
    Q2groupGdeffence = russiadeffence;
    FQ2groupG = "Russia";
    Q2groupGf = frussia;
    Q2groupGcost = russiacost;
    Q2groupGpop = russiapop;
    Q2groupG5 = russia5;
    Q2groupGC5 = russiaC5;
    Q2groupGV5 = russiaV5;
    Q2groupGD5 = russiaD5;
    FR1game1T = "Russia";
}
else if (russia < argentina && russia > france && russia > turkey) {
    cout << "Russia is the second of Group G" << endl;
    Q2groupG = russia;
    Q2groupGattack = russiaattack;
    Q2groupGmidfield = russiamidfield;
    Q2groupGdeffence = russiadeffence;
    FQ2groupG = "Russia";
    Q2groupGf = frussia;
    Q2groupGcost = russiacost;
    Q2groupGpop = russiapop;
    Q2groupG5 = russia5;
    Q2groupGC5 = russiaC5;
    Q2groupGV5 = russiaV5;
    Q2groupGD5 = russiaD5;
}
else {}

//turkey
if (turkey > argentina && turkey > france && turkey < russia) {
    cout << "Turkey is the second of Group G" << endl;
    Q2groupG = turkey;
    Q2groupGattack = turkeyattack;
    Q2groupGmidfield = turkeymidfield;
    Q2groupGdeffence = turkeydeffence;
    FQ2groupG = "Turkey";
    Q2groupGf = fturkey;
    Q2groupGcost = turkeycost;
    Q2groupGpop = turkeypop;
    Q2groupG5 = turkey5;
    Q2groupGC5 = turkeyC5;
    Q2groupGV5 = turkeyV5;
    Q2groupGD5 = turkeyD5;
}
else if (turkey > argentina && turkey < france && turkey > russia) {
    cout << "Turkey is the second of Group G" << endl;
    Q2groupG = turkey;
    Q2groupGattack = turkeyattack;
    Q2groupGmidfield = turkeymidfield;
    Q2groupGdeffence = turkeydeffence;
    FQ2groupG = "Turkey";
    Q2groupGf = fturkey;
    Q2groupGcost = turkeycost;
    Q2groupGpop = turkeypop;
    Q2groupG5 = turkey5;
    Q2groupGC5 = turkeyC5;
    Q2groupGV5 = turkeyV5;
    Q2groupGD5 = turkeyD5;
}
else if (turkey < argentina && turkey > france && turkey > russia) {
    cout << "Turkey is the second of Group G" << endl;
    Q2groupG = turkey;
    Q2groupGattack = turkeyattack;
    Q2groupGmidfield = turkeymidfield;
    Q2groupGdeffence = turkeydeffence;
    FQ2groupG = "Turkey";
    Q2groupGf = fturkey;
    Q2groupGcost = turkeycost;
    Q2groupGpop = turkeypop;
    Q2groupG5 = turkey5;
    Q2groupGC5 = turkeyC5;
    Q2groupGV5 = turkeyV5;
    Q2groupGD5 = turkeyD5;
}
else {}
    
    //There are many if statements for this because every team's individual statistic is competing with every team's individual statistic.

    //group F

 //attack of romania
 if (romaniaattack > icelandattack) {
     romania += 5;
 }
 if (romaniaattack > englandattack) {
     romania += 5;
 }
 if (romaniaattack > spainattack) {
     romania += 5;
 }

 //attack of iceland
 if (icelandattack > romaniaattack) {
     iceland += 5;
 }
 if (icelandattack > englandattack) {
     iceland += 5;
 }
 if (icelandattack > spainattack) {
     iceland += 5;
 }

 //attack of england
 if (englandattack > romaniaattack) {
     england += 5;
 }
 if (englandattack > icelandattack) {
     england += 5;
 }
 if (englandattack > spainattack) {
     england += 5;
 }

 //attack of spain
 if (spainattack > romaniaattack) {
     spain += 5;
 }
 if (spainattack > englandattack) {
     spain += 5;
 }
 if (spainattack > icelandattack) {
     spain += 5;
 }

 //midfield of romania
 if (romaniamidfield > englandmidfield) {
     romania += 5;
 }
 if (romaniamidfield > icelandmidfield) {
     romania += 5;
 }
 if (romaniamidfield > spainmidfield) {
     romania += 5;
 }
 
 //midfield of england
 if (englandmidfield > romaniamidfield) {
     england += 5;
 }
 if (englandmidfield > icelandmidfield) {
     england += 5;
 }
 if (englandmidfield > spainmidfield) {
     england += 5;
 }

 //midfield of iceland
 if (icelandmidfield > romaniamidfield) {
     iceland += 5;
 }
 if (icelandmidfield > englandmidfield) {
     iceland += 5;
 }
 if (icelandmidfield > spainmidfield) {
     iceland += 5;
 }

 //midfield of spain
 if (spainmidfield > romaniamidfield) {
     spain += 5;
 }
 if (spainmidfield > englandmidfield) {
     spain += 5;
 }
 if (spainmidfield > icelandmidfield) {
     spain += 5;
 } 

 //defense of romania
 if (romaniadeffence > englanddeffence) {
     romania += 5;
 }
 if (romaniadeffence > icelanddeffence) {
     romania += 5;
 }
 if (romaniadeffence > spaindeffence) {
     romania += 5;
 }

 //defense of england
 if (englanddeffence > romaniadeffence) {
     england += 5;
 }
 if (englanddeffence > icelanddeffence) {
     england += 5;
 }
 if (englanddeffence > spaindeffence) {
     england += 5;
 }

 //defense of iceland
 if (icelanddeffence > romaniadeffence) {
     iceland += 5;
 }
 if (icelanddeffence > englanddeffence) {
     iceland += 5;
 }
 if (icelanddeffence > spaindeffence) {
     iceland += 5;
 }

 //defense of spain
 if (spaindeffence > romaniadeffence) {
     spain += 5;
 }
 if (spaindeffence > englanddeffence) {
     spain += 5;
 }
 if (spaindeffence > icelanddeffence) {
     spain += 5;
 } 

 //cost of spain
    if (spaincost > romaniacost) {
    spain += 3;
}

    if (spaincost > englandcost) {
    spain += 3;
}

    if (spaincost > icelandcost) {
    spain += 3;
}

//cost of romania
    if (romaniacost > spaincost) {
    romania += 3;
}

    if (romaniacost > englandcost) {
    romania += 3;
}

    if (romaniacost > icelandcost) {
    romania += 3;
}

//cost of england
    if (englandcost > spaincost) {
    england += 3;
}

    if (englandcost > romaniacost) {
    england += 3;
}

    if (englandcost > icelandcost) {
    england += 3;
}

//cost of iceland
    if (icelandcost > spaincost) {
    iceland += 3;
}

    if (icelandcost > englandcost) {
    iceland += 3;
}

    if (icelandcost > romaniacost) {
    iceland += 3;
}

//population of spain
if (spainpop > romaniapop) {
    spain += 3;
}

if (spainpop > englandpop) {
    spain += 3;
}

if (spainpop > icelandpop) {
    spain += 3;
}

//population of england
if (englandpop > romaniapop) {
    england+= 3;
}

if (englandpop > spainpop) {
    england += 3;
}

if (englandpop > icelandpop) {
    england += 3;
}

//population of iceland
if (icelandpop > romaniapop) {
    iceland+= 3;
}

if (icelandpop > spainpop) {
    iceland += 3;
}

if (icelandpop > englandpop) {
    iceland += 3;
}

//population of romania
if (romaniapop > englandpop) {
    romania += 3;
}

if (romaniapop > spainpop) {
    romania += 3;
}

if (romaniapop > icelandpop) {
    romania += 3;
}

//spain # of goals score in last 5 games
if (spain5 > england5) {
    spain += 1;
}

if (spain5 > romania5) {
    spain += 1;
}

if (spain5 > iceland5) {
    spain += 1;
}

//england # of goals score in last 5 games
if (england5 > romania5) {
    england += 1;
}

if (england5 > spain5) {
    england += 1;
}

if (england5 > iceland5) {
    england += 1;
}

//iceland # of goals score in last 5 games
if (iceland5 > romania5) {
    iceland += 1;
}

if (iceland5 > spain5) {
    iceland += 1;
}

if (iceland5 > england5) {
    iceland += 1;
}

//romania # of goals score in last 5 games
if (romania5 > iceland5) {
    romania += 1;
}

if (romania5 > spain5) {
    romania += 1;
}

if (romania5 > england5) {
    romania += 1;
}

//spain # of goals conceded in last 5 games
if (spainC5 > romaniaC5) {
    spain -= 1;
}

if (spainC5 > englandC5) {
    spain -= 1;
}

if (spainC5 > icelandC5) {
    spain -= 1;
}

//england # of goals conceded in last 5 games
if (englandC5 > romaniaC5) {
    england -= 1;
}

if (englandC5 > spainC5) {
    england -= 1;
}

if (englandC5 > icelandC5) {
    england -= 1;
}

//romania # of goals conceded in last 5 games
if (romaniaC5 > englandC5) {
    romania -= 1;
}

if (romaniaC5 > spainC5) {
    romania -= 1;
}

if (romaniaC5 > icelandC5) {
    romania -= 1;
}

//iceland # of goals conceded in last 5 games
if (icelandC5 > englandC5) {
    iceland -= 1;
}

if (icelandC5 > spainC5) {
    iceland -= 1;
}

if (icelandC5 > romaniaC5) {
    iceland -= 1;
}

//spain # of goals victory in last 5 games
if (spainV5 > englandV5) {
    spain += 1;
}

if (spainV5 > icelandV5) {
    spain += 1;
}

if (spainV5 > romaniaV5) {
    spain += 1;
}

//england # of goals victory in last 5 games
if (englandV5 > spainV5) {
    england += 1;
}

if (englandV5 > icelandV5) {
    england += 1;
}

if (englandV5 > romaniaV5) {
    england += 1;
}

//iceland # of goals victory in last 5 games
if (icelandV5 > spainV5) {
    iceland += 1;
}

if (icelandV5 > englandV5) {
    iceland += 1;
}

if (icelandV5 > romaniaV5) {
    iceland += 1;
}

//romania # of goals victory in last 5 games
if (romaniaV5 > spainV5) {
    romania += 1;
}

if (romaniaV5 > englandV5) {
    romania += 1;
}

if (romaniaV5 > icelandV5) {
    romania += 1;
}

//spain # of goals defeat in last 5 games
if (spainD5 > englandD5) {
    spain -= 1;
}

if (spainD5 > romaniaD5) {
    spain -= 1;
}

if (spainD5 > icelandD5) {
    spain -= 1;
}

//england # of goals defeat in last 5 games
if (englandD5 > spainD5) {
    england -= 1;
}

if (englandD5 > romaniaD5) {
    england -= 1;
}

if (englandD5 > icelandD5) {
    england -= 1;
}

//iceland # of goals defeat in last 5 games
if (icelandD5 > spainD5) {
    iceland -= 1;
}

if (icelandD5 > romaniaD5) {
    iceland -= 1;
}

if (icelandD5 > englandD5) {
    iceland -= 1;
}

//romania # of goals defeat in last 5 games
if (romaniaD5 > spainD5) {
    romania -= 1;
}

if (romaniaD5 > icelandD5) {
    romania -= 1;
}

if (romaniaD5 > englandD5) {
    romania -= 1;
}

//spain factor of unexpectancy
if (fspain > fromania) {
    spain = spain + r9;
}

if (fspain > ficeland) {
    spain = spain + r9;
}

if (fspain > fengland) {
    spain = spain + r9;
}

//england factor of unexpectancy
if (fengland > fromania) {
    england = england + r10;
}

if (fengland > ficeland) {
    england = england + r10;
}

if (fengland > fspain) {
    england = england + r10;
}

//iceland factor of unexpectancy
if (ficeland > fromania) {
    iceland = iceland + r11;
}

if (ficeland > fengland) {
    iceland = iceland + r11;
}

if (ficeland > fspain) {
    iceland = iceland + r11;
}

//romania factor of unexpectancy
if (fromania > ficeland) {
    romania = romania + r12;
}

if (fromania > fengland) {
    romania = romania + r12;
}

if (fromania > fspain) {
    romania = romania + r12;
}


 //1st place results of group F
 if (spain > romania && spain > england && spain > iceland) {
    cout << "Spain is the winner of Group F" << endl;
    Q1groupF = spain;
    Q1groupFattack = spainattack;
    Q1groupFmidfield = spainmidfield;
    Q1groupFdeffence = spaindeffence;
    FQ1groupF = "Spain";
    Q1groupFf = fspain;
    Q1groupFcost = spaincost;
    Q1groupFpop = spainpop;
    Q1groupF5 = spain5;
    Q1groupFC5 = spainC5;
    Q1groupFV5 = spainV5;
    Q1groupFD5 = spainD5;
}
else if (romania > spain && romania > england && romania > iceland) {
    cout << "Romania is the winner of Group F" << endl;
    Q1groupF = romania;
    Q1groupFattack = romaniaattack;
    Q1groupFmidfield = romaniamidfield;
    Q1groupFdeffence = romaniadeffence;
    FQ1groupF = "Romania";
    Q1groupFf = fromania;
    Q1groupFcost = romaniacost;
    Q1groupFpop = romaniapop;
    Q1groupF5 = romania5;
    Q1groupFC5 = romaniaC5;
    Q1groupFV5 = romaniaV5;
    Q1groupFD5 = romaniaD5;
}
else if (england > spain && england > romania && england > iceland) {
    cout << "England is the winner of Group F" << endl;
    Q1groupF = england;
    Q1groupFattack = englandattack;
    Q1groupFmidfield = englandmidfield;
    Q1groupFdeffence = englanddeffence;
    FQ1groupF = "England";
    Q1groupFf = fengland;
    Q1groupFcost = englandcost;
    Q1groupFpop = englandpop;
    Q1groupF5 = england5;
    Q1groupFC5 = englandC5;
    Q1groupFV5 = englandV5;
    Q1groupFD5 = englandD5;
}
else if (iceland > spain && iceland > england && iceland > romania) {
    cout << "Iceland is the winner of Group F" << endl;
    Q1groupF = iceland;
    Q1groupFattack = icelandattack;
    Q1groupFmidfield = icelandmidfield;
    Q1groupFdeffence = icelanddeffence;
    FQ1groupF = "Iceland";
    Q1groupFf = ficeland;
    Q1groupFcost = icelandcost;
    Q1groupFpop = icelandpop;
    Q1groupF5 = iceland5;
    Q1groupFC5 = icelandC5;
    Q1groupFV5 = icelandV5;
    Q1groupFD5 = icelandD5;
}

//2nd place winner of group F

//Spain
if (spain > iceland && spain > england && spain < romania) {
    cout << "Spain is the second of Group F" << endl;
    Q2groupF = spain;
    Q2groupFattack = spainattack;
    Q2groupFmidfield = spainmidfield;
    Q2groupFdeffence = spaindeffence;
    FQ2groupF = "Spain";
    Q2groupFf = fspain;
    Q2groupFcost = spaincost;
    Q2groupFpop = spainpop;
    Q2groupF5 = spain5;
    Q2groupFC5 = spainC5;
    Q2groupFV5 = spainV5;
    Q2groupFD5 = spainD5;
}
else if (spain > iceland && spain < england && spain > romania) {
    cout << "Spain is the second of Group F" << endl;
    Q2groupF = spain;
    Q2groupFattack = spainattack;
    Q2groupFmidfield = spainmidfield;
    Q2groupFdeffence = spaindeffence;
    FQ2groupF = "Spain";
    Q2groupFf = fspain;
    Q2groupFcost = spaincost;
    Q2groupFpop = spainpop;
    Q2groupF5 = spain5;
    Q2groupFC5 = spainC5;
    Q2groupFV5 = spainV5;
    Q2groupFD5 = spainD5;
}
else if (spain < iceland && spain > england && spain > england) {
    cout << "Spain is the second of Group F" << endl;
    Q2groupF = spain;
    Q2groupFattack = spainattack;
    Q2groupFmidfield = spainmidfield;
    Q2groupFdeffence = spaindeffence;
    FQ2groupF = "Spain";
    Q2groupFf = fspain;
    Q2groupFcost = spaincost;
    Q2groupFpop = spainpop;
    Q2groupF5 = spain5;
    Q2groupFC5 = spainC5;
    Q2groupFV5 = spainV5;
    Q2groupFD5 = spainD5;
}
else {}

//Iceland
if (iceland > spain && iceland > england && iceland < romania) {
    cout << "Iceland is the second of Group F" << endl;
    Q2groupF = iceland;
    Q2groupFattack = icelandattack;
    Q2groupFmidfield = icelandmidfield;
    Q2groupFdeffence = icelanddeffence;
    FQ2groupF = "Iceland";
    Q2groupFf = ficeland;
    Q2groupFcost = icelandcost;
    Q2groupFpop = icelandpop;
    Q2groupF5 = iceland5;
    Q2groupFC5 = icelandC5;
    Q2groupFV5 = icelandV5;
    Q2groupFD5 = icelandD5;
}
else if (iceland > spain && iceland < england && iceland > romania) {
     cout << "Iceland is the second of Group F" << endl;
    Q2groupF = iceland;
    Q2groupFattack = icelandattack;
    Q2groupFmidfield = icelandmidfield;
    Q2groupFdeffence = icelanddeffence;
    FQ2groupF = "Iceland";
    Q2groupFf = ficeland;
    Q2groupFcost = icelandcost;
    Q2groupFpop = icelandpop;
    Q2groupF5 = iceland5;
    Q2groupFC5 = icelandC5;
    Q2groupFV5 = icelandV5;
    Q2groupFD5 = icelandD5;
}
else if (iceland < spain && iceland > england && iceland > romania) {
     cout << "Iceland is the second of Group F" << endl;
    Q2groupF = iceland;
    Q2groupFattack = icelandattack;
    Q2groupFmidfield = icelandmidfield;
    Q2groupFdeffence = icelanddeffence;
    FQ2groupF = "Iceland";
    Q2groupFf = ficeland;
    Q2groupFcost = icelandcost;
    Q2groupFpop = icelandpop;
    Q2groupF5 = iceland5;
    Q2groupFC5 = icelandC5;
    Q2groupFV5 = icelandV5;
    Q2groupFD5 = icelandD5;
}
else {}

//England
if (england > spain && england > iceland && england < romania) {
    cout << "England is the second of Group F" << endl;
    Q2groupF = england;
    Q2groupFattack = englandattack;
    Q2groupFmidfield = englandmidfield;
    Q2groupFdeffence = englanddeffence;
    FQ2groupF = "England";
    Q2groupFf = fengland;
    Q2groupFcost = englandcost;
    Q2groupFpop = englandpop;
    Q2groupF5 = england5;
    Q2groupFC5 = englandC5;
    Q2groupFV5 = englandV5;
    Q2groupFD5 = englandD5;
}
else if (england > spain && england < iceland && england > romania) {
     cout << "England is the second of Group F" << endl;
    Q2groupF = england;
    Q2groupFattack = englandattack;
    Q2groupFmidfield = englandmidfield;
    Q2groupFdeffence = englanddeffence;
    FQ2groupF = "England";
    Q2groupFf = fengland;
    Q2groupFcost = englandcost;
    Q2groupFpop = englandpop;
    Q2groupF5 = england5;
    Q2groupFC5 = englandC5;
    Q2groupFV5 = englandV5;
    Q2groupFD5 = englandD5;
}
else if (england < spain && england > iceland && england > romania) {
     cout << "England is the second of Group F" << endl;
    Q2groupF = england;
    Q2groupFattack = englandattack;
    Q2groupFmidfield = englandmidfield;
    Q2groupFdeffence = englanddeffence;
    FQ2groupF = "England";
    Q2groupFf = fengland;
    Q2groupFcost = englandcost;
    Q2groupFpop = englandpop;
    Q2groupF5 = england5;
    Q2groupFC5 = englandC5;
    Q2groupFV5 = englandV5;
    Q2groupFD5 = englandD5;
}
else {}

//romania
if (romania > spain && romania > iceland && romania < england) {
    cout << "Romania is the second of Group F" << endl;
    Q2groupF = romania;
    Q2groupFattack = romaniaattack;
    Q2groupFmidfield = romaniamidfield;
    Q2groupFdeffence = romaniadeffence;
    FQ2groupF = "Romania";
    Q2groupFf = fromania;
    Q2groupFcost = romaniacost;
    Q2groupFpop = romaniapop;
    Q2groupF5 = romania5;
    Q2groupFC5 = romaniaC5;
    Q2groupFV5 = romaniaV5;
    Q2groupFD5 = romaniaD5;
}
else if (romania > spain && romania < iceland && romania > england) {
     cout << "Romania is the second of Group F" << endl;
    Q2groupF = romania;
    Q2groupFattack = romaniaattack;
    Q2groupFmidfield = romaniamidfield;
    Q2groupFdeffence = romaniadeffence;
    FQ2groupF = "Romania";
    Q2groupFf = fromania;
    Q2groupFcost = romaniacost;
    Q2groupFpop = romaniapop;
    Q2groupF5 = romania5;
    Q2groupFC5 = romaniaC5;
    Q2groupFV5 = romaniaV5;
    Q2groupFD5 = romaniaD5;
}
else if (romania < spain && romania > iceland && romania > england) {
     cout << "Romania is the second of Group F" << endl;
    Q2groupF = romania;
    Q2groupFattack = romaniaattack;
    Q2groupFmidfield = romaniamidfield;
    Q2groupFdeffence = romaniadeffence;
    FQ2groupF = "Romania";
    Q2groupFf = fromania;
    Q2groupFcost = romaniacost;
    Q2groupFpop = romaniapop;
    Q2groupF5 = romania5;
    Q2groupFC5 = romaniaC5;
    Q2groupFV5 = romaniaV5;
    Q2groupFD5 = romaniaD5;
}
else {}

    //There are many if statements for this because every team's individual statistic is competing with every team's individual statistic.
    
    //group E

    //attack of brazil
if (brazilattack > germanyattack) {
    brazil += 5;
}
if (brazilattack > senegalattack) {
    brazil += 5;
}
if (brazilattack > austriaattack) {
    brazil += 5;
}

//attack of germany
if (germanyattack > brazilattack) {
    germany += 5;
} 
if (germanyattack > senegalattack) {
    germany += 5;
} 
if (germanyattack > austriaattack) {
    germany += 5;
} 

//attack of senegal
if (senegalattack > brazilattack) {
    senegal += 5;
}
if (senegalattack > germanyattack) {
    senegal += 5;
}
if (senegalattack > austriaattack) {
    senegal += 5;
}

//attack of austria
if (austriaattack > brazilattack) {
    austria += 5;
} 
if (austriaattack > germanyattack) {
    austria += 5;
}
if (austriaattack > senegalattack) {
    austria += 5;
} 

//midfield of brazil 
if (brazilmidfield > germanymidfield) {
    brazil += 5;
}
if (brazilmidfield > senegalmidfield) {
    brazil += 5;
}
if (brazilmidfield > austriamidfield) {
    brazil += 5;
}

//midfield of germany
if (germanymidfield > brazilmidfield) {
    germany += 5;
}
if (germanymidfield > senegalmidfield) {
    germany += 5;
}
if (germanymidfield > austriamidfield) {
    germany += 5;
}

//midfield of senegal
if (senegalmidfield > brazilmidfield) {
    senegal += 5;
}
if (senegalmidfield > germanymidfield) {
    senegal += 5;
}
if (senegalmidfield > austriamidfield) {
    senegal += 5;
}

//midfield of austria
if (austriamidfield > brazilmidfield) {
    austria += 5;
}
if (austriamidfield > germanymidfield) {
    austria += 5;
}
if (austriamidfield > senegalmidfield) {
    austria += 5;
}

//defense of brazil
if (brazildeffence > germanydeffence) {
    brazil += 5;
}
if (brazildeffence > senegaldeffence) {
    brazil += 5;
}
if (brazildeffence > austriadeffence) {
    brazil += 5;
}

//defense of germany
if (germanydeffence > brazildeffence) {
    germany += 5;
}
if (germanydeffence > senegaldeffence) {
    germany += 5;
}
if (germanydeffence > austriadeffence) {
    germany += 5;
}

//defense of senegal 
if (senegaldeffence > brazildeffence) {
    senegal += 5;
}
if (senegaldeffence > germanydeffence) {
    senegal += 5;
}
if (senegaldeffence > austriadeffence) {
    senegal += 5;
}

//defense of austria
if (austriadeffence > brazildeffence) {
    austria += 5;
}
if (austriadeffence > germanydeffence) {
    austria += 5;
}
if (austriadeffence > senegaldeffence) {
    austria += 5;
}

//cost of brazil
    if (brazilcost > germanycost) {
    brazil += 3;
}

    if (brazilcost > senegalcost) {
    brazil += 3;
}

    if (brazilcost > austriacost) {
    brazil += 3;
}

//cost of germany
    if (germanycost > brazilcost) {
    germany += 3;
}

    if (germanycost > senegalcost) {
    germany += 3;
}

    if (germanycost > austriacost) {
    germany += 3;
}

//cost of senegal
    if (senegalcost > brazilcost) {
    senegal += 3;
}

    if (senegalcost > germanycost) {
    senegal += 3;
}

    if (senegalcost > austriacost) {
    senegal += 3;
}

//cost of austria
    if (austriacost > brazilcost) {
    austria += 3;
}

    if (austriacost > germanycost) {
    austria += 3;
}

    if (austriacost > senegalcost) {
    austria += 3;
}

//population of brazil
if (brazilpop > germanypop) {
    brazil += 3;
}

if (brazilpop > senegalpop) {
    brazil += 3;
}

if (brazilpop > austriapop) {
    brazil += 3;
}

//population of germany
if (germanypop > brazilpop) {
    germany += 3;
}

if (germanypop > senegalpop) {
    germany += 3;
}

if (germanypop > austriapop) {
    germany += 3;
}

//population of senegal
if (senegalpop > brazilpop) {
    senegal += 3;
}

if (senegalpop > germanypop) {
    senegal += 3;
}

if (senegalpop > austriapop) {
    senegal += 3;
}

//population of austria
if (austriapop > brazilpop) {
    austria += 3;
}

if (austriapop > germanypop) {
    austria += 3;
}

if (austriapop > senegalpop) {
    austria += 3;
}

//brazil # of goals score in last 5 games
if (brazil5 > germany5) {
    brazil += 1;
}

if (brazil5 > senegal5) {
    brazil += 1;
}

if (brazil5 > austria5) {
    brazil += 1;
}

//germany # of goals score in last 5 games
if (germany5 > brazil5) {
    germany += 1;
}

if (germany5 > senegal5) {
    germany += 1;
}

if (germany5 > austria5) {
    germany += 1;
}

//senegal # of goals score in last 5 games
if (senegal5 > brazil5) {
    senegal += 1;
}

if (senegal5 > germany5) {
    senegal += 1;
}

if (senegal5 > austria5) {
    senegal += 1;
}

//austria # of goals score in last 5 games
if (austria5 > brazil5) {
    austria += 1;
}

if (austria5 > germany5) {
    austria += 1;
}

if (austria5 > senegal5) {
    austria += 1;
}

//brazil # of goals conceded in last 5 games
if (brazilC5 > germanyC5) {
    brazil -= 1;
}

if (brazilC5 > senegalC5) {
    brazil -= 1;
}

if (brazilC5 > austriaC5) {
    brazil -= 1;
}

//germany # of goals conceded in last 5 games
if (germanyC5 > brazilC5) {
    germany -= 1;
}

if (germanyC5 > senegalC5) {
    germany -= 1;
}

if (germanyC5 > austriaC5) {
    germany -= 1;
}

//senegal # of goals conceded in last 5 games
if (senegalC5 > brazilC5) {
    senegal -= 1;
}

if (senegalC5 > germanyC5) {
    senegal -= 1;
}

if (senegalC5 > austriaC5) {
    senegal -= 1;
}

//austria # of goals conceded in last 5 games
if (austriaC5 > brazilC5) {
    austria -= 1;
}

if (austriaC5 > germanyC5) {
    austria -= 1;
}

if (austriaC5 > senegalC5) {
    austria -= 1;
}

//brazil # of goals victory in last 5 games
if (brazilV5 > germanyV5) {
    brazil += 1;
}

if (brazilV5 > senegalV5) {
    brazil += 1;
}

if (brazilV5 > austriaV5) {
    brazil += 1;
}

//germany # of goals victory in last 5 games
if (germanyV5 > brazilV5) {
    germany += 1;
}

if (germanyV5 > senegalV5) {
    germany += 1;
}

if (germanyV5 > austriaV5) {
    germany += 1;
}

//senegal # of goals victory in last 5 games
if (senegalV5 > brazilV5) {
    senegal += 1;
}

if (senegalV5 > germanyV5) {
    senegal += 1;
}

if (senegalV5 > austriaV5) {
    senegal += 1;
}

//austria # of goals victory in last 5 games
if (austriaV5 > brazilV5) {
    austria += 1;
}

if (austriaV5 > senegalV5) {
    austria += 1;
}

if (austriaV5 > germany5) {
    austria += 1;
}

//brazil # of goals defeat in last 5 games
if (brazilD5 > germanyD5) {
    brazil -= 1;
}

if (brazilD5 > senegalD5) {
    brazil -= 1;
}

if (brazilD5 > austriaD5) {
    brazil -= 1;
}

//germany # of goals defeat in last 5 games
if (germanyD5 > brazilD5) {
    germany -= 1;
}

if (germanyD5 > senegalD5) {
    germany -= 1;
}

if (germanyD5 > austriaD5) {
    germany -= 1;
}

//senegal # of goals defeat in last 5 games
if (senegalD5 > brazilD5) {
    senegal -= 1;
}

if (senegalD5 > germanyD5) {
    senegal -= 1;
}

if (senegalD5 > austriaD5) {
    senegal -= 1;
}

//austria # of goals defeat in last 5 games
if (austriaD5 > brazilD5) {
    austria -= 1;
}

if (austriaD5 > germanyD5) {
    austria -= 1;
}

if (austriaD5 > austriaD5) {
    austria -= 1;
}

//brazil factor of unexpectancy
if (fbrazil > fgermany) {
    brazil = brazil + r13;
}

if (fbrazil > fsenegal) {
    brazil = brazil + r13;
}

if (fbrazil > faustria) {
    brazil = brazil + r13;
}

//germany factor of unexpectancy
if (fgermany > fbrazil) {
    germany = germany + r14;
}

if (fgermany > fsenegal) {
    germany = germany + r14;
}

if (fgermany > faustria) {
    germany = germany + r14;
}

//senegal factor of unexpectancy
if (fsenegal > fbrazil) {
    senegal = senegal + r15;
}

if (fsenegal > fgermany) {
    senegal = senegal + r15;
}

if (fsenegal > faustria) {
    senegal = senegal + r15;
}

//austria factor of unexpectancy
if (faustria > fbrazil) {
    austria = austria + r16;
}

if (faustria > fgermany) {
    austria = austria + r16;
}

if (faustria > fsenegal) {
    austria = austria + r16;
}


//1st place results of group E
if (brazil > germany && brazil > austria && brazil > senegal) {
        cout << "Brazil is the winner of Group E" << endl;
        Q1groupE = brazil;
        Q1groupEattack = brazilattack;
        Q1groupEmidfield = brazilmidfield;
        Q1groupEdeffence = brazildeffence;
        FQ1groupE = "Brazil";
        Q1groupEf = fbrazil;
        Q1groupEcost = brazilcost;
        Q1groupEpop = brazilpop;
        Q1groupE5 = brazil5;
        Q1groupEC5 = brazilC5;
        Q1groupEV5 = brazilV5;
        Q1groupED5 = brazilD5;
    }
    else if (germany > brazil && germany > austria && germany > senegal) {
        cout << "Germany is the winner of Group E" << endl;
        Q1groupE = germany;
        Q1groupEattack = germanyattack;
        Q1groupEmidfield = germanymidfield;
        Q1groupEdeffence = germanydeffence;
        FQ1groupE = "Germany";
        Q1groupEf = fgermany;
        Q1groupEcost = germanycost;
        Q1groupEpop = germanypop;
        Q1groupE5 = germany5;
        Q1groupEC5 = germanyC5;
        Q1groupEV5 = germanyV5;
        Q1groupED5 = germanyD5;
    }
    else if (austria > brazil && austria > germany && austria > senegal) {
        cout << "Austria is the winner of Group E" << endl;
        Q1groupE = austria;
        Q1groupEattack = austriaattack;
        Q1groupEmidfield = austriamidfield;
        Q1groupEdeffence = austriadeffence;
        FQ1groupE = "Austria";
        Q1groupEf = faustria;
        Q1groupEcost = austriacost;
        Q1groupEpop = austriapop;
        Q1groupE5 = austria5;
        Q1groupEC5 = austriaC5;
        Q1groupEV5 = austriaV5;
        Q1groupED5 = austriaD5;
    }
    else if (senegal > germany && senegal > brazil && senegal > austria) {
        cout << "Senegal is the winner of Group E" << endl;
        Q1groupE = senegal;
        Q1groupEattack = senegalattack;
        Q1groupEmidfield = senegalmidfield;
        Q1groupEdeffence = senegaldeffence;
        FQ1groupE = "Senegal";
        Q1groupEf = fsenegal;
        Q1groupEcost = senegalcost;
        Q1groupEpop = senegalpop;
        Q1groupE5 = senegal5;
        Q1groupEC5 = senegalC5;
        Q1groupEV5 = senegalV5;
        Q1groupED5 = senegalD5;
    }
    else {}

    
//2nd place result of group E

//Brazil

if (brazil > germany && brazil > senegal && brazil < austria) {
    cout << "Brazil is the second of Group E" << endl;
    Q2groupE = brazil;
    Q2groupEattack = brazilattack;
    Q2groupEmidfield = brazilmidfield;
    Q2groupEdeffence = brazildeffence;
    FQ2groupE = "Brazil";
    Q2groupEf = fbrazil;
    Q2groupEcost = brazilcost;
    Q2groupEpop = brazilpop;
    Q2groupE5 = brazil5;
    Q2groupEC5 = brazilC5;
    Q2groupEV5 = brazilV5;
    Q2groupED5 = brazilD5;
}
else if (brazil > germany && brazil < senegal && brazil > austria) {
    cout << "Brazil is the second of Group E" << endl;
    Q2groupE = brazil;
    Q2groupEattack = brazilattack;
    Q2groupEmidfield = brazilmidfield;
    Q2groupEdeffence = brazildeffence;
    FQ2groupE = "Brazil";
    Q2groupEf = fbrazil;
    Q2groupEcost = brazilcost;
    Q2groupEpop = brazilpop;
    Q2groupE5 = brazil5;
    Q2groupEC5 = brazilC5;
    Q2groupEV5 = brazilV5;
    Q2groupED5 = brazilD5;
}
else if (brazil < germany && brazil > senegal && brazil > austria) {
    cout << "Brazil is the second of Group E" << endl;
    Q2groupE = brazil;
    Q2groupEattack = brazilattack;
    Q2groupEmidfield = brazilmidfield;
    Q2groupEdeffence = brazildeffence;
    FQ2groupE = "Brazil";
    Q2groupEf = fbrazil;
    Q2groupEcost = brazilcost;
    Q2groupEpop = brazilpop;
    Q2groupE5 = brazil5;
    Q2groupEC5 = brazilC5;
    Q2groupEV5 = brazilV5;
    Q2groupED5 = brazilD5;
}
else {}

//Germany
if (germany > brazil && germany > senegal && germany < austria) {
    cout << "Germany is the second of Group E" << endl;
    Q2groupE = germany;
    Q2groupEattack = germanyattack;
    Q2groupEmidfield = germanymidfield;
    Q2groupEdeffence = germanydeffence;
    FQ2groupE = "Germany";
    Q2groupEf = fgermany;
    Q2groupEcost = germanycost;
    Q2groupEpop = germanypop;
    Q2groupE5 = germany5;
    Q2groupEC5 = germanyC5;
    Q2groupEV5 = germanyV5;
    Q2groupED5 = germanyD5;
}
else if (germany > brazil && germany < senegal && germany > austria) {
     cout << "Germany is the second of Group E" << endl;
    Q2groupE = germany;
    Q2groupEattack = germanyattack;
    Q2groupEmidfield = germanymidfield;
    Q2groupEdeffence = germanydeffence;
    FQ2groupE = "Germany";
    Q2groupEf = fgermany;
    Q2groupEcost = germanycost;
    Q2groupEpop = germanypop;
    Q2groupE5 = germany5;
    Q2groupEC5 = germanyC5;
    Q2groupEV5 = germanyV5;
    Q2groupED5 = germanyD5;
}
else if (germany < brazil && germany > senegal && germany > austria) {
     cout << "Germany is the second of Group E" << endl;
    Q2groupE = germany;
    Q2groupEattack = germanyattack;
    Q2groupEmidfield = germanymidfield;
    Q2groupEdeffence = germanydeffence;
    FQ2groupE = "Germany";
    Q2groupEf = fgermany;
    Q2groupEcost = germanycost;
    Q2groupEpop = germanypop;
    Q2groupE5 = germany5;
    Q2groupEC5 = germanyC5;
    Q2groupEV5 = germanyV5;
    Q2groupED5 = germanyD5;
}
else {}

//Senegal
if (senegal > brazil && senegal > germany && senegal < austria) {
    cout << "Senegal is the second of Group E" << endl;
    Q2groupE = senegal;
    Q2groupEattack = senegalattack;
    Q2groupEmidfield = senegalmidfield;
    Q2groupEdeffence = senegaldeffence;
    FQ2groupE = "Senegal";
    Q2groupEf = fsenegal;
    Q2groupEcost = senegalcost;
    Q2groupEpop = senegalpop;
    Q2groupE5 = senegal5;
    Q2groupEC5 = senegalC5;
    Q2groupEV5 = senegalV5;
    Q2groupED5 = senegalD5;
}
else if (senegal > brazil && senegal < germany && senegal > austria) {
     cout << "Senegal is the second of Group E" << endl;
    Q2groupE = senegal;
    Q2groupEattack = senegalattack;
    Q2groupEmidfield = senegalmidfield;
    Q2groupEdeffence = senegaldeffence;
    FQ2groupE = "Senegal";
    Q2groupEf = fsenegal;
    Q2groupEcost = senegalcost;
    Q2groupEpop = senegalpop;
    Q2groupE5 = senegal5;
    Q2groupEC5 = senegalC5;
    Q2groupEV5 = senegalV5;
    Q2groupED5 = senegalD5;
}
else if (senegal < brazil && senegal > germany && senegal > austria) {
   cout << "Senegal is the second of Group E" << endl;
    Q2groupE = senegal;
    Q2groupEattack = senegalattack;
    Q2groupEmidfield = senegalmidfield;
    Q2groupEdeffence = senegaldeffence;
    FQ2groupE = "Senegal";
    Q2groupEf = fsenegal;
    Q2groupEcost = senegalcost;
    Q2groupEpop = senegalpop;
    Q2groupE5 = senegal5;
    Q2groupEC5 = senegalC5;
    Q2groupEV5 = senegalV5;
    Q2groupED5 = senegalD5;
}
else {}

//Austria
if (austria > brazil && austria > germany && austria < senegal) {
    cout << "Austria is the second of Group E" << endl;
    Q2groupE = austria;
    Q2groupEattack = austriaattack;
    Q2groupEmidfield = austriamidfield;
    Q2groupEdeffence = austriadeffence;
    FQ2groupE = "Austria";
    Q2groupEf = faustria;
    Q2groupEcost = austriacost;
    Q2groupEpop = austriapop;
    Q2groupE5 = austria5;
    Q2groupEC5 = austriaC5;
    Q2groupEV5 = austriaV5;
    Q2groupED5 = austriaD5;
}
else if (austria > brazil && austria < germany && austria > senegal) {
     cout << "Austria is the second of Group E" << endl;
    Q2groupE = austria;
    Q2groupEattack = austriaattack;
    Q2groupEmidfield = austriamidfield;
    Q2groupEdeffence = austriadeffence;
    FQ2groupE = "Austria";
    Q2groupEf = faustria;
    Q2groupEcost = austriacost;
    Q2groupEpop = austriapop;
    Q2groupE5 = austria5;
    Q2groupEC5 = austriaC5;
    Q2groupEV5 = austriaV5;
    Q2groupED5 = austriaD5;
}
else if (austria < brazil && austria > germany && austria > senegal) {
   cout << "Austria is the second of Group E" << endl;
    Q2groupE = austria;
    Q2groupEattack = austriaattack;
    Q2groupEmidfield = austriamidfield;
    Q2groupEdeffence = austriadeffence;
    FQ2groupE = "Austria";
    Q2groupEf = faustria;
    Q2groupEcost = austriacost;
    Q2groupEpop = austriapop;
    Q2groupE5 = austria5;
    Q2groupEC5 = austriaC5;
    Q2groupEV5 = austriaV5;
    Q2groupED5 = austriaD5;
}
else {}
    
    //There are many if statements for this because every team's individual statistic is competing with every team's individual statistic.

    //group D


    //attack of wales
    if (walesattack > polandattack) {
        wales += 5;
    }
    if (walesattack > usaattack) {
        wales += 5;
    }
    if (walesattack > peruattack) {
        wales += 5;
    }

    //attack of poland
    if (polandattack > walesattack) {
        poland += 5;
    }
    if (polandattack > usaattack) {
        poland += 5;
    }
    if (polandattack > peruattack) {
        poland += 5;
    }

    //attack of usa
    if (usaattack > walesattack) {
        usa += 5;
    }
    if (usaattack > polandattack) {
        usa += 5;
    }
    if (usaattack > peruattack) {
        usa += 5;
    }

    //attack of peru
    if (peruattack > usaattack) {
        peru += 5;
    }
    if (peruattack > polandattack) {
        peru += 5;
    }
    if (peruattack > walesattack) {
        peru += 5;
    }

    //midfield of wales
    if (walesmidfield > usamidfield) {
        wales += 5;
    }
    if (walesmidfield > polandmidfield) {
        wales += 5;
    }
    if (walesmidfield > perumidfield) {
        wales += 5;
    }

    //midfield of usa
    if (usamidfield > walesmidfield) {
        usa += 5;
    }
    if (usamidfield > polandmidfield) {
        usa += 5;
    }
    if (usamidfield > perumidfield) {
        usa += 5;
    } 

    //midfield of peru
    if (perumidfield > walesmidfield) {
        peru += 5;
    }
    if (perumidfield > usamidfield) {
        peru += 5;
    }
    if (perumidfield > polandmidfield) {
        peru += 5;
    } 

    //midfield of poland
    if (polandmidfield > walesmidfield) {
        poland += 5;
    }
    if (polandmidfield > usamidfield) {
        poland += 5;
    }
    if (polandmidfield > perumidfield) {
        poland += 5;
    }
    
    //defense of wales
    if (walesdeffence > usadeffence) {
        wales += 5;
    }
    if (walesdeffence > polanddeffence) {
        wales += 5;
    }
    if (walesdeffence > perudeffence) {
        wales += 5;
    }

    //defense of usa
    if (usadeffence > polanddeffence) {
        usa += 5;
    }
    if (usadeffence > walesdeffence) {
        usa += 5;
    }
    if (usadeffence > perudeffence) {
        usa += 5;
    }

    //defense of poland
    if (polanddeffence > walesdeffence) {
        poland += 5;
    } 
    if (polanddeffence > usadeffence) {
        poland += 5;
    } 
    if (polanddeffence > perudeffence) {
        poland += 5;
    } 

    //defense of peru
    if (perudeffence > walesdeffence) {
        peru += 5;
    }
    if (perudeffence > usadeffence) {
        peru += 5;
    }
    if (perudeffence > polanddeffence) {
        peru += 5;
    }

    //cost of poland
    if (polandcost > walescost) {
    poland += 3;
}

    if (polandcost > usacost) {
    poland += 3;
}

if (polandcost > perucost) {
    poland += 3;
}

//cost of peru
if (perucost > walescost) {
    peru += 3;
}

if (perucost > usacost) {
    peru += 3;
}

if (perucost > polandcost) {
    peru += 3;
}

//cost of usa
if (usacost > polandcost) {
    usa += 3;
}

if (usacost > perucost) {
    usa += 3;
}

if (usacost > walescost) {
    netherlands += 3;
}

//cost of wales
if (walescost > polandcost) {
    wales += 3;
}

if (walescost > usacost) {
    wales += 3;
}

if (walescost > perucost) {
    wales += 3;
}

//population of wales
if (walespop > polandpop) {
    wales += 3;
}

if (walespop > perupop) {
    wales += 3;
}

if (walespop > usapop) {
    wales += 3;
}

//population of poland
if (polandpop > walespop) {
    poland += 3;
}

if (polandpop > usapop) {
    poland += 3;
}

if (polandpop > perupop) {
    poland += 3;
}

//population of usa
if (usapop > walespop) {
    usa += 3;
}

if (usapop > perupop) {
    usa += 3;
}

if (usapop > polandpop) {
    usa += 3;
}

//population of peru
if (perupop > walespop) {
    peru += 3;
}

if (perupop > polandpop) {
    peru += 3;
}

if (perupop > usapop) {
    peru += 3;
}

//wales # of goals score in last 5 games
if (wales5 > usa5) {
    wales += 1;
}

if (wales5 > peru5) {
    wales += 1;
}

if (wales5 > poland5) {
    wales += 1;
}

//poland # of goals score in last 5 games
if (poland5 > peru5) {
    poland += 1;
}

if (poland5 > usa5) {
    poland += 1;
}

if (poland5 > wales5) {
    poland += 1;
}

//usa # of goals score in last 5 games
if (usa5 > poland5) {
    usa += 1;
}

if (usa5 > peru5) {
    usa += 1;
}

if (usa5 > wales5) {
    usa += 1;
}

//peru # of goals score in last 5 games
if (peru5 > usa5) {
    peru += 1;
}

if (peru5 > poland5) {
    peru += 1;
}

if (peru5 > wales5) {
    peru += 1;
}

//wales # of goals conceded in last 5 games
if (walesC5 > polandC5) {
    wales -= 1;
}

if (walesC5 > peruC5) {
    wales -= 1;
}

if (walesC5 > usaC5) {
    wales -= 1;
}

//usa # of goals conceded in last 5 games
if (usaC5 > walesC5) {
    usa -= 1;
}

if (usaC5 > polandC5) {
    usa -= 1;
}

if (usaC5 > peruC5) {
    usa -= 1;
}

//poland # of goals conceded in last 5 games
if (polandC5 > peruC5) {
    poland -= 1;
}

if (polandC5 > walesC5) {
    poland -= 1;
}

if (polandC5 > usaC5) {
    poland -= 1;
}

//peru # of goals conceded in last 5 games
if (peruC5 > polandC5) {
    peru -= 1;
}

if (peruC5 > usaC5) {
    peru -= 1;
}

if (peruC5 > walesC5) {
    peru -= 1;
}

//wales # of goals victory in last 5 games
if (walesV5 > polandV5) {
    wales += 1;
}

if (walesV5 > peruV5) {
    wales += 1;
}

if (walesV5 > usaV5) {
    wales += 1;
}

//usa # of goals victory in last 5 games
if (usaV5 > polandV5) {
    usa += 1;
}

if (usaV5 > peruV5) {
    usa += 1;
}

if (usaV5 > wales5) {
    usa += 1;
}

//poland # of goals victory in last 5 games
if (polandV5 > usaV5) {
    poland += 1;
}

if (polandV5 > peruV5) {
    poland += 1;
}

if (polandV5 > walesV5) {
    poland += 1;
}

//peru # of goals victory in last 5 games
if (peruV5 > usaV5) {
    peru += 1;
}

if (peruV5 > peruV5) {
    peru += 1;
}

if (peruV5 > walesV5) {
    peru += 1;
}

//wales # of goals defeat in last 5 games
if (walesD5 > polandD5) {
    wales -= 1;
}

if (walesD5 > peruD5) {
    wales -= 1;
}

if (walesD5 > usaD5) {
    wales -= 1;
}

//usa # of goals defeat in last 5 games
if (usaD5 > polandD5) {
    usa -= 1;
}

if (usaD5 > peruD5) {
    usa -= 1;
}

if (usaD5 > walesD5) {
    usa -= 1;
}

//poland # of goals defeat in last 5 games
if (polandD5 > usaD5) {
    poland -= 1;
}

if (polandD5 > peruD5) {
    poland -= 1;
}

if (polandD5 > walesD5) {
    poland -= 1;
}

//peru # of goals defeat in last 5 games
if (peruD5 > usaD5) {
    peru -= 1;
}

if (peruD5 > polandD5) {
    peru -= 1;
}

if (peruD5 > walesD5) {
    peru -= 1;
}

//factor of unexpectancy of peru
if (fperu > fusa) {
    peru = peru + r17;
}

if (fperu > fpoland) {
    peru = peru + r17;
}

if (fperu > walesD5) {
    peru = peru + r17;
}

//factor of unexpectancy of usa
if (fusa > fperu) {
    usa = usa + r18;
}

if (fusa > fpoland) {
    usa = usa + r18;
}

if (fusa > walesD5) {
    usa = usa + r18;
}

//factor of unexpectancy of poland
if (fpoland > fperu) {
    poland = poland + r19;
}

if (fpoland > fusa) {
    poland = poland + r19;
}

if (fpoland > walesD5) {
    poland = poland + r19;
}

//factor of unexpectancy of wales
if (walesD5 > fperu) {
    wales = wales + r20;
}

if (walesD5 > fusa) {
    wales = wales + r20;
}

if (walesD5 > fpoland) {
    wales = wales + r20;
}

    //1st place results of group D
     if (peru > wales && peru > usa && peru > poland) {
        cout << "Peru is the winner of Group D" << endl;
        Q1groupD = peru;
        Q1groupDattack = peruattack;
        Q1groupDmidfield = perumidfield;
        Q1groupDdeffence = perudeffence;
        FQ1groupD = "Peru";
        Q1groupDf = fperu;
        Q1groupDcost = perucost;
        Q1groupDpop = perupop;
        Q1groupD5 = peru5;
        Q1groupDC5 = peruC5;
        Q1groupDV5 = peruV5;
        Q1groupDD5 = peruD5;
    }
    else if (wales > peru && wales > usa && wales > poland) {
        cout << "Wales is the winner of Group D" << endl;
        Q1groupD = wales;
        Q1groupDattack = walesattack;
        Q1groupDmidfield = walesmidfield;
        Q1groupDdeffence = walesdeffence;
        FQ1groupD = "Wales";
        Q1groupDf = fwales;
        Q1groupDcost = walescost;
        Q1groupDpop = walespop;
        Q1groupD5 = wales5;
        Q1groupDC5 = walesC5;
        Q1groupDV5 = walesV5;
        Q1groupDD5 = walesD5;
    }
    else if (usa > wales && usa > peru && usa > poland) {
        cout << "USA is the winner of Group D" << endl;
        Q1groupD = usa;
        Q1groupDattack = usaattack;
        Q1groupDmidfield = usamidfield;
        Q1groupDdeffence = usadeffence;
        FQ1groupD = "USA";
        Q1groupDf = fusa;
        Q1groupDcost = usacost;
        Q1groupDpop = usapop;
        Q1groupD5 = usa5;
        Q1groupDC5 = usaC5;
        Q1groupDV5 = usaV5;
        Q1groupDD5 = usaD5;
    }
    else if (poland > wales && poland > peru && poland > usa) {
        cout << "Poland is the winner of Group D" << endl;
        Q1groupD = poland;
        Q1groupDattack = polandattack;
        Q1groupDmidfield = polandmidfield;
        Q1groupDdeffence = polanddeffence;
        FQ1groupD = "poland";
        Q1groupDf = fpoland;
        Q1groupDcost = polandcost;
        Q1groupDpop = polandpop;
        Q1groupD5 = poland5;
        Q1groupDC5 = polandC5;
        Q1groupDV5 = polandV5;
        Q1groupDD5 = polandD5;
    }
    else {}

    //2nd place results of group D
    ////////////////////////////////
    
    //peru 

    if (peru > wales && peru > usa && peru < poland) {
        cout << "Peru is the second of Group D" << endl;
        Q2groupD = peru;
        Q2groupDattack = peruattack;
        Q2groupDmidfield = perumidfield;
        Q2groupDdeffence = perudeffence;
        FQ2groupD = "Peru";
        Q2groupDf = fperu;
        Q2groupDcost = perucost;
        Q2groupDpop = perupop;
        Q2groupD5 = peru5;
        Q2groupDC5 = peruC5;
        Q2groupDV5 = peruV5;
        Q2groupDD5 = peruD5;
    }
    else if (peru > wales && peru < usa && peru > poland) {
         cout << "Peru is the second of Group D" << endl;
        Q2groupD = peru;
        Q2groupDattack = peruattack;
        Q2groupDmidfield = perumidfield;
        Q2groupDdeffence = perudeffence;
        FQ2groupD = "Peru";
        Q2groupDf = fperu;
        Q2groupDcost = perucost;
        Q2groupDpop = perupop;
        Q2groupD5 = peru5;
        Q2groupDC5 = peruC5;
        Q2groupDV5 = peruV5;
        Q2groupDD5 = peruD5;
    }
    else if (peru < wales && peru > usa && peru > poland) {
       cout << "Peru is the second of Group D" << endl;
        Q2groupD = peru;
        Q2groupDattack = peruattack;
        Q2groupDmidfield = perumidfield;
        Q2groupDdeffence = perudeffence;
        FQ2groupD = "Peru";
        Q2groupDf = fperu;
        Q2groupDcost = perucost;
        Q2groupDpop = perupop;
        Q2groupD5 = peru5;
        Q2groupDC5 = peruC5;
        Q2groupDV5 = peruV5;
        Q2groupDD5 = peruD5;
    }
    else {}

    //wales
    if (wales > peru && wales > usa && wales < poland) {
        cout << "Wales is the second of Group D" << endl;
        Q2groupD = wales;
        Q2groupDattack = walesattack;
        Q2groupDmidfield = walesmidfield;
        Q2groupDdeffence = walesdeffence;
        FQ2groupD = "Wales";
        Q2groupDf = fwales;
        Q2groupDcost = walescost;
        Q2groupDpop = walespop;
        Q2groupD5 = wales5;
        Q2groupDC5 = walesC5;
        Q2groupDV5 = walesV5;
        Q2groupDD5 = walesD5;
    }
    else if (wales > peru && wales < usa && wales > poland) {
         cout << "Wales is the second of Group D" << endl;
        Q2groupD = wales;
        Q2groupDattack = walesattack;
        Q2groupDmidfield = walesmidfield;
        Q2groupDdeffence = walesdeffence;
        FQ2groupD = "Wales";
        Q2groupDf = fwales;
        Q2groupDcost = walescost;
        Q2groupDpop = walespop;
        Q2groupD5 = wales5;
        Q2groupDC5 = walesC5;
        Q2groupDV5 = walesV5;
        Q2groupDD5 = walesD5;
    }
    else if (wales < peru && wales > usa && wales > poland) {
       cout << "Wales is the second of Group D" << endl;
        Q2groupD = wales;
        Q2groupDattack = walesattack;
        Q2groupDmidfield = walesmidfield;
        Q2groupDdeffence = walesdeffence;
        FQ2groupD = "Wales";
        Q2groupDf = fwales;
        Q2groupDcost = walescost;
        Q2groupDpop = walespop;
        Q2groupD5 = wales5;
        Q2groupDC5 = walesC5;
        Q2groupDV5 = walesV5;
        Q2groupDD5 = walesD5;
    }
    else {}

    //usa
    if (usa > peru && usa > wales && usa < poland) {
        cout << "USA is the second of Group D" << endl;
        Q2groupD = usa;
        Q2groupDattack = usaattack;
        Q2groupDmidfield = usamidfield;
        Q2groupDdeffence = usadeffence;
        FQ2groupD = "USA";
        Q2groupDf = fusa;
        Q2groupDcost = usacost;
        Q2groupDpop = usapop;
        Q2groupD5 = usa5;
        Q2groupDC5 = usaC5;
        Q2groupDV5 = usaV5;
        Q2groupDD5 = usaD5;
    }
    else if (usa > peru && usa < wales && usa > poland) {
         cout << "USA is the second of Group D" << endl;
        Q2groupD = usa;
        Q2groupDattack = usaattack;
        Q2groupDmidfield = usamidfield;
        Q2groupDdeffence = usadeffence;
        FQ2groupD = "USA";
        Q2groupDf = fusa;
        Q2groupDcost = usacost;
        Q2groupDpop = usapop;
        Q2groupD5 = usa5;
        Q2groupDC5 = usaC5;
        Q2groupDV5 = usaV5;
        Q2groupDD5 = usaD5;
    }
    else if (usa < peru && usa > wales && usa > poland) {
       cout << "USA is the second of Group D" << endl;
        Q2groupD = usa;
        Q2groupDattack = usaattack;
        Q2groupDmidfield = usamidfield;
        Q2groupDdeffence = usadeffence;
        FQ2groupD = "USA";
        Q2groupDf = fusa;
        Q2groupDcost = usacost;
        Q2groupDpop = usapop;
        Q2groupD5 = usa5;
        Q2groupDC5 = usaC5;
        Q2groupDV5 = usaV5;
        Q2groupDD5 = usaD5;
    }
    else {}

    //poland
    if (poland > peru && poland > wales && poland < usa) {
        cout << "Poland is the second of Group D" << endl;
        Q2groupD = poland;
        Q2groupDattack = polandattack;
        Q2groupDmidfield = polandmidfield;
        Q2groupDdeffence = polanddeffence;
        FQ2groupD = "Poland";
        Q2groupDf = fpoland;
        Q2groupDcost = polandcost;
        Q2groupDpop = polandpop;
        Q2groupD5 = poland5;
        Q2groupDC5 = polandC5;
        Q2groupDV5 = polandV5;
        Q2groupDD5 = polandD5;
    }
    else if (poland > peru && poland < wales && poland > usa) {
         cout << "Poland is the second of Group D" << endl;
        Q2groupD = poland;
        Q2groupDattack = polandattack;
        Q2groupDmidfield = polandmidfield;
        Q2groupDdeffence = polanddeffence;
        FQ2groupD = "Poland";
        Q2groupDf = fpoland;
        Q2groupDcost = polandcost;
        Q2groupDpop = polandpop;
        Q2groupD5 = poland5;
        Q2groupDC5 = polandC5;
        Q2groupDV5 = polandV5;
        Q2groupDD5 = polandD5;
    }
    else if (poland < peru && poland > wales && poland > usa) {
       cout << "Poland is the second of Group D" << endl;
        Q2groupD = poland;
        Q2groupDattack = polandattack;
        Q2groupDmidfield = polandmidfield;
        Q2groupDdeffence = polanddeffence;
        FQ2groupD = "Poland";
        Q2groupDf = fpoland;
        Q2groupDcost = polandcost;
        Q2groupDpop = polandpop;
        Q2groupD5 = poland5;
        Q2groupDC5 = polandC5;
        Q2groupDV5 = polandV5;
        Q2groupDD5 = polandD5;
    }
    else {}
    
    //There are many if statements for this because every team's individual statistic is competing with every team's individual statistic.

    //group C

    //attack of chile
    if (chileattack > swedenattack) {
        chile += 5;
    } 
    
    if (chileattack > netherlandsattack) {
        chile += 5;
    }
    
    if (chileattack > mexicoattack) {
        chile += 5;
    } 
    
    //attack of sweden
    if (swedenattack > chileattack) {
        sweden += 5;
    }
    
    if (swedenattack > netherlandsattack) {
        sweden += 5;
    } 
    
    if (swedenattack > mexicoattack) {
        sweden += 5;
    } 
     
    //attack of netherlands
    if (netherlandsattack > swedenattack) {
        netherlands += 5;
    }
     
     if (netherlandsattack > chileattack) {
        netherlands += 5;
    } 
    
    if (netherlandsattack > mexicoattack) {
        netherlands += 5;
    }
    
    
    //attack of mexico
    if (mexicoattack > chileattack) {
        mexico += 5;
    }
    
    if (mexicoattack > swedenattack) {
        mexico += 5;
    }
    
    if (mexicoattack > netherlandsattack) {
        mexico += 5;
    }
    
    //midfield of chile
    if (chilemidfield > swedenmidfield) {
        chile += 5;
    }
    
    if (chilemidfield > netherlandsmidfield) {
        chile += 5;
    }
    
    if (chilemidfield > mexicomidfield) {
        chile += 5;
    }
     
    //midfield of sweden
    if (swedenmidfield > chilemidfield) {
        sweden += 5;
    } 
    if (swedenmidfield > netherlandsmidfield) {
        sweden += 5;
    }
    if (swedenmidfield > mexicomidfield) {
        sweden += 5;
    }
    
    //midfield of netherlands
    if (netherlandsmidfield > chilemidfield) {
        netherlands += 5;
    }
    if (netherlandsmidfield > swedenmidfield) {
        netherlands += 5;
    }
    if (netherlandsmidfield > mexicomidfield) {
        netherlands += 5;
    } 
    
    //midfield of mexico 
    if (mexicomidfield > chilemidfield) {
        mexico += 5;
    }
    if (mexicomidfield > swedenmidfield) {
        mexico += 5;
    }
    if (mexicomidfield > netherlandsmidfield) {
        mexico += 5;
    }
    
    //defense of chile
    if (chiledeffence > swedendeffence) {
        chile += 5;
    }
    if (chiledeffence > netherlandsdeffence) {
        chile += 5;
    }
    if (chiledeffence > mexicodeffence) {
        chile += 5;
    }
     
     //defense of sweden
     if (swedendeffence > chiledeffence) {
         sweden += 5;
     }
     if (swedendeffence > netherlandsdeffence) {
         sweden += 5;
     }
     if (swedendeffence > mexicodeffence) {
         sweden += 5;
     }
     
     //defense of netherlands
     if (netherlandsdeffence > chiledeffence) {
         netherlands += 5;
     }
     if (netherlandsdeffence > swedendeffence) {
         netherlands += 5;
     }
     if (netherlandsdeffence > mexicodeffence) {
         netherlands += 5;
     }
     
     //defense of mexico
     if (mexicodeffence > chiledeffence) {
         mexico += 5;
     }
     if (mexicodeffence > swedendeffence) {
         mexico += 5;
     }
     if (mexicodeffence > netherlandsdeffence) {
         mexico += 5;
     }

     //cost of mexico
    if (mexicocost > chilecost) {
    mexico += 3;
}

    if (mexicocost > swedencost) {
    mexico += 3;
}

if (mexicocost > netherlandscost) {
    mexico += 3;
}

//cost of chile
if (chilecost > mexicocost) {
    chile += 3;
}

if (chilecost > swedencost) {
    chile += 3;
}

if (chilecost > netherlandscost) {
    chile += 3;
}

//cost of netherlands
if (netherlandscost > mexicocost) {
    netherlands += 3;
}

if (netherlandscost > swedencost) {
    netherlands += 3;
}

if (netherlandscost > chilecost) {
    netherlands += 3;
}

//cost of sweden
if (swedencost > chilecost) {
    sweden += 3;
}

if (swedencost > netherlandscost) {
    sweden += 3;
}

if (swedencost > mexicocost) {
    sweden += 3;
}

//population of chile
if (chilepop > netherlandspop) {
    chile += 3;
}

if (chilepop > mexicopop) {
    chile += 3;
}

if (chilepop > swedenpop) {
    chile += 3;
}

//population of mexico
if (mexicopop > chilepop) {
    mexico += 3;
}

if (mexicopop > netherlandspop) {
    mexico += 3;
}

if (mexicopop > swedenpop) {
    mexico += 3;
}

//population of sweden
if (swedenpop > chilepop) {
    sweden += 3;
}

if (swedenpop > netherlandspop) {
    sweden += 3;
}

if (swedenpop > mexicopop) {
    sweden += 3;
}

//population of netherlands
if (netherlandspop > chilepop) {
    netherlands += 3;
}

if (netherlandspop > swedenpop) {
    netherlands += 3;
}

if (netherlandspop > mexicopop) {
    netherlands += 3;
}

//chile # of goals score in last 5 games
if (chile5 > sweden5) {
    chile += 1;
}

if (chile5 > netherlands5) {
    chile += 1;
}

if (chile5 > mexico5) {
    chile += 1;
}

//netherlands # of goals score in last 5 games
if (netherlands5 > chile5) {
    netherlands += 1;
}

if (netherlands5 > sweden5) {
    netherlands += 1;
}

if (netherlands5 > mexico5) {
    netherlands += 1;
}

//sweden # of goals score in last 5 games
if (sweden5 > netherlands5) {
    sweden += 1;
}

if (sweden5 > chile5) {
    sweden += 1;
}

if (sweden5 > mexico5) {
    sweden += 1;
}

//mexico # of goals score in last 5 games
if (mexico5 > chile5) {
    mexico += 1;
}

if (mexico5 > sweden5) {
    mexico += 1;
}

if (mexico5 > netherlands5) {
    mexico += 1;
}

//chile # of goals conceded in last 5 games
if (chileC5 > mexicoC5) {
    chile -= 1;
}

if (chileC5 > netherlandsC5) {
    chile -= 1;
}

if (chileC5 > swedenC5) {
    chile -= 1;
}

//sweden # of goals conceded in last 5 games
if (swedenC5 > chileC5) {
    sweden -= 1;
}

if (swedenC5 > netherlandsC5) {
    sweden -= 1;
}

if (swedenC5 > mexicoC5) {
    sweden -= 1;
}

//netherlands # of goals conceded in last 5 games
if (netherlandsC5 > chileC5) {
    portugal -= 1;
}

if (netherlandsC5 > swedenC5) {
    netherlands -= 1;
}

if (netherlandsC5 > mexicoC5) {
    netherlands -= 1;
}

//mexico # of goals conceded in last 5 games
if (mexicoC5 > chileC5) {
    mexico -= 1;
}

if (mexicoC5 > swedenC5) {
    mexico -= 1;
}

if (mexicoC5 > netherlandsC5) {
    mexico -= 1;
}

//chile # of goals victory in last 5 games
if (chileV5 > netherlandsV5) {
    chile += 1;
}

if (chileV5 > swedenV5) {
    chile += 1;
}

if (chileV5 > mexicoV5) {
    chile += 1;
}

//sweden # of goals victory in last 5 games
if (swedenV5 > netherlandsV5) {
    sweden += 1;
}

if (swedenV5 > chileV5) {
    sweden += 1;
}

if (swedenV5 > mexicoV5) {
    sweden += 1;
}

//netherlands # of goals victory in last 5 games
if (netherlandsV5 > chileV5) {
    netherlands += 1;
}

if (netherlandsV5 > mexicoV5) {
    netherlands += 1;
}

if (netherlandsV5 > swedenV5) {
    netherlands += 1;
}

//mexico # of goals victory in last 5 games
if (mexicoV5 > chileV5) {
    mexico += 1;
}

if (mexicoV5 > netherlandsV5) {
    mexico += 1;
}

if (mexicoV5 > swedenV5) {
    mexico += 1;
}

//chile # of defeats in last 5 games
if (chileD5 > mexicoD5) {
    chile -= 1;
}

if (chileD5 > netherlandsD5) {
    chile -= 1;
}

if (chileD5 > swedenD5) {
    chile -= 1;
}

//netherlands # of defeats in last 5 games
if (netherlandsD5 > chileD5) {
    netherlands -= 1;
}

if (netherlandsD5 > mexicoD5) {
    netherlands -= 1;
}

if (netherlandsD5 > swedenD5) {
    netherlands -= 1;
}

//mexico # of defeats in last 5 games
if (mexicoD5 > chileD5) {
    mexico -= 1;
}

if (mexicoD5 > swedenD5) {
    mexico -= 1;
}

if (mexicoD5 > netherlandsD5) {
    mexico -= 1;
}

//sweden # of defeats in last 5 games
if (swedenD5 > chileD5) {
    sweden -= 1;
}

if (swedenD5 > mexicoD5) {
    sweden -= 1;
}

if (swedenD5 > netherlandsD5) {
    sweden -= 1;
}

//chile factor of unexpectancy
if (fchile > fsweden) {
    chile = chile + r21;
}

if (fchile > fnetherlands) {
    chile = chile + r21;
}

if (fchile > fmexico) {
    chile = chile + r21;
}

//sweden factor of unexpectancy
if (fsweden > fchile) {
    sweden = sweden + r22;
}

if (fsweden > fnetherlands) {
    sweden = sweden + r22;
}

if (fsweden > fmexico) {
    sweden = sweden + r22;
}

//netherlands factor of unexpectancy
if (fnetherlands > fchile) {
    netherlands = netherlands + r23;
}

if (fnetherlands > fmexico) {
    netherlands = netherlands + r23;
}

if (fnetherlands > fsweden) {
    netherlands = netherlands + r23;
}

//mexico factor of unexpectancy
if (fmexico > fchile) {
    mexico = mexico + r24;
}

if (fmexico > fnetherlands) {
    mexico = mexico + r24;
}

if (fmexico > fsweden) {
    mexico = mexico + r24;
}


     //first place results of group C
     if (chile > netherlands && chile > sweden && chile > mexico) {
        cout << "Chile is the winner of Group C" << endl;
        Q1groupC = chile;
        Q1groupCattack = chileattack;
        Q1groupCmidfield = chilemidfield;
        Q1groupCdeffence = chiledeffence;
        FQ1groupC = "Chile";
        Q1groupCf = fchile;
        Q1groupCcost = chilecost;
        Q1groupCpop = chilepop;
        Q1groupC5 = chile5;
        Q1groupCC5 = chileC5;
        Q1groupCV5 = chileV5;
        Q1groupCD5 = chileD5;
        
    }
     else if (netherlands > chile && netherlands > sweden && netherlands > mexico) {
        cout << "Netherlands is the winner of Group C" << endl;
        Q1groupC = netherlands;
        Q1groupCattack = netherlandsattack;
        Q1groupCmidfield = netherlandsmidfield;
        Q1groupCdeffence = netherlandsdeffence;
        FQ1groupC = "Netherlands";
        Q1groupCf = fnetherlands;
        Q1groupCcost = netherlandscost;
        Q1groupCpop = netherlandspop;
        Q1groupC5 = netherlands5;
        Q1groupCC5 = netherlandsC5;
        Q1groupCV5 = netherlandsV5;
        Q1groupCD5 = netherlandsD5;
        
    }
    else if (sweden > chile && sweden > netherlands && sweden > mexico) {
        cout << "Sweden is the winner of Group C" << endl;
        Q1groupC = sweden;
        Q1groupCattack = swedenattack;
        Q1groupCmidfield = swedenmidfield;
        Q1groupCdeffence = swedendeffence;
        FQ1groupC = "Sweden";
        Q1groupCf = fsweden;
        Q1groupCcost = swedencost;
        Q1groupCpop = swedenpop;
        Q1groupC5 = sweden5;
        Q1groupCC5 = swedenC5;
        Q1groupCV5 = swedenV5;
        Q1groupCD5 = swedenD5;
        
    }
    else if (mexico > chile && mexico > sweden && mexico > netherlands) {
        cout << "Mexico is the winner of Group C" << endl;
        Q1groupC = mexico;
        Q1groupCattack = mexicoattack;
        Q1groupCmidfield = mexicomidfield;
        Q1groupCdeffence = mexicodeffence;
        FQ1groupC = "Mexico";
        Q1groupCf = fmexico;
        Q1groupCcost = mexicocost;
        Q1groupCpop = mexicopop;
        Q1groupC5 = mexico5;
        Q1groupCC5 = mexicoC5;
        Q1groupCV5 = mexicoV5;
        Q1groupCD5 = mexicoD5;
        
    }
    else {}

    //2nd place result of group C

    //mexico
    if (mexico > chile && mexico > sweden && mexico < netherlands) {
        cout << "Mexico is the second of Group C" << endl;
        Q2groupC = mexico;
        Q2groupCattack = mexicoattack;
        Q2groupCmidfield = mexicomidfield;
        Q2groupCdeffence = mexicodeffence;
        FQ2groupC = "Mexico";
        Q2groupCf = fmexico;
        Q2groupCcost = mexicocost;
        Q2groupCpop = mexicopop;
        Q2groupC5 = mexico5;
        Q2groupCC5 = mexicoC5;
        Q2groupCV5 = mexicoV5;
        Q2groupCD5 = mexicoD5;
    }
    else if (mexico > chile && mexico < sweden && mexico > netherlands) {
         cout << "Mexico is the second of Group C" << endl;
        Q2groupC = mexico;
        Q2groupCattack = mexicoattack;
        Q2groupCmidfield = mexicomidfield;
        Q2groupCdeffence = mexicodeffence;
        FQ2groupC = "Mexico";
        Q2groupCf = fmexico;
        Q2groupCcost = mexicocost;
        Q2groupCpop = mexicopop;
        Q2groupC5 = mexico5;
        Q2groupCC5 = mexicoC5;
        Q2groupCV5 = mexicoV5;
        Q2groupCD5 = mexicoD5;
    }
    else if (mexico < chile && mexico > sweden && mexico > netherlands) {
       cout << "Mexico is the second of Group C" << endl;
        Q2groupC = mexico;
        Q2groupCattack = mexicoattack;
        Q2groupCmidfield = mexicomidfield;
        Q2groupCdeffence = mexicodeffence;
        FQ2groupC = "Mexico";
        Q2groupCf = fmexico;
        Q2groupCcost = mexicocost;
        Q2groupCpop = mexicopop;
        Q2groupC5 = mexico5;
        Q2groupCC5 = mexicoC5;
        Q2groupCV5 = mexicoV5;
        Q2groupCD5 = mexicoD5;
    }
    else {}

    //chile
    if (chile > mexico && chile > sweden && chile < netherlands) {
        cout << "Chile is the second of Group C" << endl;
        Q2groupC = chile;
        Q2groupCattack = chileattack;
        Q2groupCmidfield = chilemidfield;
        Q2groupCdeffence = chiledeffence;
        FQ2groupC = "Chile";
        Q2groupCf = fchile;
        Q2groupCcost = chilecost;
        Q2groupCpop = chilepop;
        Q2groupC5 = chile5;
        Q2groupCC5 = chileC5;
        Q2groupCV5 = chileV5;
        Q2groupCD5 = chileD5;
    }
    else if (chile > mexico && chile < sweden && chile > netherlands) {
         cout << "Chile is the second of Group C" << endl;
        Q2groupC = chile;
        Q2groupCattack = chileattack;
        Q2groupCmidfield = chilemidfield;
        Q2groupCdeffence = chiledeffence;
        FQ2groupC = "Chile";
        Q2groupCf = fchile;
        Q2groupCcost = chilecost;
        Q2groupCpop = chilepop;
        Q2groupC5 = chile5;
        Q2groupCC5 = chileC5;
        Q2groupCV5 = chileV5;
        Q2groupCD5 = chileD5;
    }
    else if (chile < mexico && mexico > sweden && mexico > netherlands) {
       cout << "Chile is the second of Group C" << endl;
        Q2groupC = chile;
        Q2groupCattack = chileattack;
        Q2groupCmidfield = chilemidfield;
        Q2groupCdeffence = chiledeffence;
        FQ2groupC = "Chile";
        Q2groupCf = fchile;
        Q2groupCcost = chilecost;
        Q2groupCpop = chilepop;
        Q2groupC5 = chile5;
        Q2groupCC5 = chileC5;
        Q2groupCV5 = chileV5;
        Q2groupCD5 = chileD5;
    }
    else {}

    //sweden

    if (sweden > mexico && sweden > chile && sweden < netherlands) {
        cout << "Sweden is the second of Group C" << endl;
        Q2groupC = sweden;
        Q2groupCattack = swedenattack;
        Q2groupCmidfield = swedenmidfield;
        Q2groupCdeffence = swedendeffence;
        FQ2groupC = "Sweden";
        Q2groupCf = fsweden;
        Q2groupCcost = swedencost;
        Q2groupCpop = swedenpop;
        Q2groupC5 = sweden5;
        Q2groupCC5 = swedenC5;
        Q2groupCV5 = swedenV5;
        Q2groupCD5 = swedenD5;
    }
    else if (sweden > mexico && sweden < chile && sweden > netherlands) {
         cout << "Sweden is the second of Group C" << endl;
        Q2groupC = sweden;
        Q2groupCattack = swedenattack;
        Q2groupCmidfield = swedenmidfield;
        Q2groupCdeffence = swedendeffence;
        FQ2groupC = "Sweden";
        Q2groupCf = fsweden;
        Q2groupCcost = swedencost;
        Q2groupCpop = swedenpop;
        Q2groupC5 = sweden5;
        Q2groupCC5 = swedenC5;
        Q2groupCV5 = swedenV5;
        Q2groupCD5 = swedenD5;
    }
    else if (sweden < mexico && sweden > mexico && sweden > netherlands) {
       cout << "Sweden is the second of Group C" << endl;
        Q2groupC = sweden;
        Q2groupCattack = swedenattack;
        Q2groupCmidfield = swedenmidfield;
        Q2groupCdeffence = swedendeffence;
        FQ2groupC = "Sweden";
        Q2groupCf = fsweden;
        Q2groupCcost = swedencost;
        Q2groupCpop = swedenpop;
        Q2groupC5 = sweden5;
        Q2groupCC5 = swedenC5;
        Q2groupCV5 = swedenV5;
        Q2groupCD5 = swedenD5;
    }
    else {} 

    //netherlands

    if (netherlands > mexico && netherlands > chile && netherlands < sweden) {
        cout << "Netherlands is the second of Group C" << endl;
        Q2groupC = netherlands;
        Q2groupCattack = netherlandsattack;
        Q2groupCmidfield = netherlandsmidfield;
        Q2groupCdeffence = netherlandsdeffence;
        FQ2groupC = "Netherlands";
        Q2groupCf = fnetherlands;
        Q2groupCcost = netherlandscost;
        Q2groupCpop = netherlandspop;
        Q2groupC5 = netherlands5;
        Q2groupCC5 = netherlandsC5;
        Q2groupCV5 = netherlandsV5;
        Q2groupCD5 = netherlandsD5;
    }
    else if (netherlands > mexico && netherlands < chile && netherlands > sweden) {
         cout << "Netherlands is the second of Group C" << endl;
        Q2groupC = netherlands;
        Q2groupCattack = netherlandsattack;
        Q2groupCmidfield = netherlandsmidfield;
        Q2groupCdeffence = netherlandsdeffence;
        FQ2groupC = "Netherlands";
        Q2groupCf = fnetherlands;
        Q2groupCcost = netherlandscost;
        Q2groupCpop = netherlandspop;
        Q2groupC5 = netherlands5;
        Q2groupCC5 = netherlandsC5;
        Q2groupCV5 = netherlandsV5;
        Q2groupCD5 = netherlandsD5;
    }
    else if (netherlands < mexico && netherlands > mexico && netherlands > sweden) {
       cout << "Netherlands is the second of Group C" << endl;
        Q2groupC = netherlands;
        Q2groupCattack = netherlandsattack;
        Q2groupCmidfield = netherlandsmidfield;
        Q2groupCdeffence = netherlandsdeffence;
        FQ2groupC = "Netherlands";
        Q2groupCf = fnetherlands;
        Q2groupCcost = netherlandscost;
        Q2groupCpop = netherlandspop;
        Q2groupC5 = netherlands5;
        Q2groupCC5 = netherlandsC5;
        Q2groupCV5 = netherlandsV5;
        Q2groupCD5 = netherlandsD5;
    }
    else {} 

    //There are many if statements for this because every team's individual statistic is competing with every team's individual statistic.

    //group B

    //attack of croatia
    if (croatiaattack > belgiumattack) {
        croatia += 5;
    }
    
    if (croatiaattack > denmarkattack) {
        croatia += 5;
    }

    if (croatiaattack > columbiaattack) {
        croatia += 5;
    }

    //attack of belgium
    if (belgiumattack > croatiaattack) {
        belgium += 5;
    }

    if (belgiumattack > denmarkattack) {
        belgium += 5;
    }

    if (belgiumattack > columbiaattack) {
        belgium += 5;
    }

    //attack of denmark
    if (denmarkattack > belgiumattack) {
        denmark += 5;
    }

    if (denmarkattack > croatiaattack) {
        denmark += 5;
    }

    if (denmarkattack > columbiaattack) {
        denmark += 5;
    }

    //attack of columbia
    if (columbiaattack > denmarkattack) {
        columbia += 5;
    }

    if (columbiaattack > belgiumattack) {
        columbia += 5;
    }

    if (columbiaattack > croatiaattack) {
        columbia += 5;
    }

    //midfield of croatia
    if (croatiamidfield > belgiummidfield) {
        croatia += 5;
    }
    
    if (croatiamidfield > denmarkmidfield) {
        croatia += 5;
    }

    if (croatiamidfield > columbiamidfield) {
        croatia += 5;
    }

    //midfield of belgium
    if (belgiummidfield > denmarkmidfield) {
        belgium += 5;
    }
    
    if (belgiummidfield > columbiamidfield) {
        belgium += 5;
    }

    if (belgiummidfield > croatiamidfield) {
        belgium += 5;
    }

    //midfield of denmark
    if (denmarkmidfield > columbiamidfield) {
        denmark += 5;
    }
    
    if (denmarkmidfield > croatiamidfield) {
        denmark += 5;
    }

    if (denmarkmidfield > belgiummidfield) {
        denmark += 5;
    }

    //midfield of columbia
    if (columbiamidfield > denmarkmidfield) {
        columbia += 5;
    }
    
    if (columbiamidfield > croatiamidfield) {
        columbia += 5;
    }

    if (columbiamidfield > belgiummidfield) {
        columbia += 5;
    }

    //deffence of denmark
    if (denmarkdeffence > croatiadeffence) {
        denmark += 5;
    }
    
    if (denmarkdeffence > belgiumdeffence) {
        denmark += 5;
    }

    if (denmarkdeffence > columbiadeffence) {
        denmark += 5;
    }

    //deffence of croatia
    if (croatiadeffence > columbiadeffence) {
        croatia += 5;
    }
    
    if (croatiadeffence > belgiumdeffence) {
        croatia += 5;
    }

    if (croatiadeffence > denmarkdeffence) {
        croatia += 5;
    }
    
    //deffence of belgium
    if (belgiumdeffence > denmarkdeffence) {
        belgium += 5;
    }
    
    if (belgiumdeffence > croatiadeffence) {
        belgium += 5;
    }

    if (belgiumdeffence > columbiadeffence) {
        belgium += 5;
    }

    //deffence of columbia
    if (columbiadeffence > belgiumdeffence) {
        columbia += 5;
    }
    
    if (columbiadeffence > croatiadeffence) {
        columbia += 5;
    }

    if (columbiadeffence > denmarkdeffence) {
        columbia += 5;
    }


    //cost of croatia
    if (croatiacost > belgiumcost) {
        croatia += 3;
    }
    
    if (croatiacost > denmarkcost) {
        croatia += 3;
    }

    if (croatiacost > columbiacost) {
        croatia += 3;
    }
    
    //cost of belgium
    if (belgiumcost > croatiacost) {
        belgium += 3;
    }
    
    if (belgiumcost > denmarkcost) {
        belgium += 3;
    }

    if (belgiumcost > columbiacost) {
        belgium += 3;
    }
    
    //cost of denmark
    if (denmarkcost > croatiacost) {
        denmark += 3;
    }
    
    if (denmarkcost > belgiumcost) {
        denmark += 3;
    }

    if (denmarkcost > columbiacost) {
        denmark += 3;
    }

    //cost of columbia
    if (columbiacost > croatiacost) {
        columbia += 3;
    }
    
    if (columbiacost > belgiumcost) {
        columbia += 3;
    }

    if (columbiacost > denmarkcost) {
        columbia += 3;
    }

    //population of columbia
    if (columbiapop > denmarkpop) {
        columbia += 3;
    }
    
    if (columbiapop > belgiumpop) {
        columbia += 3;
    }

    if (columbiapop > croatiapop) {
        columbia += 3;
    }

    //population of denmark
    if (denmarkpop > columbiapop) {
        denmark += 3;
    }
    
    if (denmarkpop > belgiumpop) {
        denmark += 3;
    }

    if (denmarkpop > croatiapop) {
        denmark += 3;
    }

    //population of belgium
    if (belgiumpop > columbiapop) {
        belgium += 3;
    }
    
    if (belgiumpop > denmarkpop) {
        belgium += 3;
    }

    if (belgiumpop > croatiapop) {
        belgium += 3;
    }

    //population of croatia
    if (croatiapop > columbiapop) {
        croatia += 3;
    }
    
    if (croatiapop > denmarkpop) {
        croatia += 3;
    }

    if (croatiapop > belgiumpop) {
        croatia += 3;
    }

    //croatia # of goals score in last 5 games
    if (croatia5 > belgium5) {
        croatia += 1;
    }
    
    if (croatia5 > denmark5) {
        croatia += 1;
    }

    if (croatia5 > columbia5) {
        croatia += 1;
    }

    //belgium # of goals score in last 5 games
    if (belgium5 > croatia5) {
        belgium += 1;
    }
    
    if (belgium5 > denmark5) {
        belgium += 1;
    }

    if (belgium5 > columbia5) {
        belgium += 1;
    }

    //denmark # of goals score in last 5 games
    if (denmark5 > croatia5) {
        denmark += 1;
    }
    
    if (denmark5 > belgium5) {
        denmark += 1;
    }

    if (denmark5 > columbia5) {
        denmark += 1;
    }

    //columbia # of goals score in last 5 games
    if (columbia5 > croatia5) {
        columbia += 1;
    }
    
    if (columbia5 > belgium5) {
        columbia += 1;
    }

    if (columbia5 > denmark5) {
        columbia += 1;
    }

    //columbia # of goals conceded in last 5 games
    if (columbiaC5 > denmarkC5) {
        columbia -= 1;
    }
    
    if (columbiaC5 > belgiumC5) {
        columbia -= 1;
    }

    if (columbiaC5 > croatiaC5) {
        columbia -= 1;
    }

    //denmark # of goals conceded in last 5 games
    if (denmarkC5 > columbiaC5) {
        denmark -= 1;
    }
    
    if (denmarkC5 > belgiumC5) {
        denmark -= 1;
    }

    if (denmarkC5 > croatiaC5) {
        denmark -= 1;
    }

    //belgium # of goals conceded in last 5 games
    if (belgiumC5 > columbiaC5) {
        belgium -= 1;
    }
    
    if (belgiumC5 > denmarkC5) {
        belgium -= 1;
    }

    if (belgiumC5 > croatiaC5) {
        belgium -= 1;
    }

    //croatia # of goals conceded in last 5 games
    if (croatiaC5 > columbiaC5) {
        croatia -= 1;
    }
    
    if (croatiaC5 > denmarkC5) {
        croatia -= 1;
    }

    if (croatiaC5 > belgiumC5) {
        croatia -= 1;
    }

    //croatia # of victories in last 5 games
    if (croatiaV5 > belgiumV5) {
        croatia += 1;
    }
    
    if (croatiaV5 > denmarkV5) {
        croatia += 1;
    }

    if (croatiaV5 > columbiaV5) {
        croatia += 1;
    }

    //belgium # of victories in last 5 games
    if (belgiumV5 > croatiaV5) {
        belgium += 1;
    }
    
    if (belgiumV5 > denmarkV5) {
        belgium += 1;
    }

    if (belgiumV5 > columbiaV5) {
        belgium += 1;
    }

    //denmark # of victories in last 5 games
    if (denmarkV5 > croatiaV5) {
        denmark += 1;
    }
    
    if (denmarkV5 > belgiumV5) {
        denmark += 1;
    }

    if (denmarkV5 > columbiaV5) {
        denmark += 1;
    }

    //columbia # of victories in last 5 games
    if (columbiaV5 > croatiaV5) {
        columbia += 1;
    }
    
    if (columbiaV5 > belgiumV5) {
        columbia += 1;
    }

    if (columbiaV5 > denmarkV5) {
        columbia += 1;
    }

    //columbia # of defeats in last 5 games
    if (columbiaD5 > denmarkD5) {
        columbia -= 1;
    }
    
    if (columbiaD5 > belgiumD5) {
        columbia -= 1;
    }

    if (columbiaD5 > croatiaD5) {
        columbia -= 1;
    }

    //denmark # of defeats in last 5 games
    if (denmarkD5 > columbiaD5) {
        denmark -= 1;
    }
    
    if (denmarkD5 > belgiumD5) {
        denmark -= 1;
    }

    if (denmarkD5 > croatiaD5) {
        denmark -= 1;
    }

    //belgium # of defeats in last 5 games
    if (belgiumD5 > columbiaD5) {
        belgium -= 1;
    }
    
    if (belgiumD5 > denmarkD5) {
        belgium -= 1;
    }

    if (belgiumD5 > croatiaD5) {
        belgium -= 1;
    }

    //croatia # of defeats in last 5 games
    if (croatiaD5 > columbiaD5) {
        croatia -= 1;
    }
    
    if (croatiaD5 > denmarkD5) {
        croatia -= 1;
    }

    if (croatiaD5 > belgiumD5) {
        croatia -= 1;
    }

    //croatia factor of unexpectancy
    if (fcroatia > fbelgium) {
        croatia = croatia + r25;
    }
    
    if (fcroatia > fdenmark) {
        croatia = croatia + r25;
    }

    if (fcroatia > fcolumbia) {
        croatia = croatia + r25;
    }

    //belgium factor of unexpectancy
    if (fbelgium > fcroatia) {
        belgium = belgium + r26;
    }
    
    if (fbelgium > fdenmark) {
        belgium = belgium + r26;
    }

    if (fbelgium > fcolumbia) {
        belgium = belgium + r26;
    }

    //denmark factor of unexpectancy
    if (fdenmark > fcroatia) {
        denmark = denmark + r27;
    }
    
    if (fdenmark > fbelgium) {
        denmark = denmark + r27;
    }

    if (fdenmark > fcolumbia) {
        denmark = denmark + r27;
    }

    //columbia factor of unexpectancy
    if (fcolumbia > fcroatia) {
        columbia = columbia + r28;
    }
    
    if (fcolumbia > fbelgium) {
        columbia = columbia + r28;
    }

    if (fcolumbia > fdenmark) {
        columbia = columbia + r28;
    }

    
    //1st place results of group B
    if (columbia > denmark && columbia > croatia && columbia > belgium) {
        cout << "Columbia is the winner of Group B" << endl;
        Q1groupB = columbia;
        Q1groupBattack = columbiaattack;
        Q1groupBmidfield = columbiamidfield;
        Q1groupBdeffence = columbiadeffence;
        Q1groupBf = fcolumbia;
        Q1groupBcost = columbiacost;
        Q1groupBpop = columbiapop;
        Q1groupB5 = columbia5;
        Q1groupBC5 = columbiaC5;
        Q1groupBV5 = columbiaV5;
        Q1groupBD5 = columbiaD5;
        FQ1groupB = "Columbia";
    }

    else if (denmark > columbia && denmark > croatia && denmark > belgium) {
        cout << "Denmark is the winner of Group B" << endl;
        Q1groupB = denmark;
        Q1groupBattack = denmarkattack;
        Q1groupBmidfield = denmarkmidfield;
        Q1groupBdeffence = denmarkdeffence;
        Q1groupBf = fdenmark;
        Q1groupBcost = denmarkcost;
        Q1groupBpop = denmarkpop;
        Q1groupB5 = denmark5;
        Q1groupBC5 = denmarkC5;
        Q1groupBV5 = denmarkV5;
        Q1groupBD5 = denmarkD5;
        FQ1groupB = "Denmark";
    }

    else if (croatia > denmark && croatia > belgium && croatia > columbia) {
        cout << "Croatia is the winner of Group B" << endl;
        Q1groupB = croatia;
        Q1groupBattack = croatiaattack;
        Q1groupBmidfield = croatiamidfield;
        Q1groupBdeffence = croatiadeffence;
        Q1groupBf = fcroatia;
        Q1groupBcost = croatiacost;
        Q1groupBpop = croatiapop;
        Q1groupB5 = croatia5;
        Q1groupBC5 = croatiaC5;
        Q1groupBV5 = croatiaV5;
        Q1groupBD5 = croatiaD5;
        FQ1groupB = "Croatia";
    }

    else if (belgium > denmark && belgium > croatia && belgium > columbia) {
        cout << "Belgium is the winner of Group B" << endl;
        Q1groupB = belgium;
        Q1groupBattack = belgiumattack;
        Q1groupBmidfield = belgiummidfield;
        Q1groupBdeffence = belgiumdeffence;
        Q1groupBf = fbelgium;
        Q1groupBcost = belgiumcost;
        Q1groupBpop = belgiumpop;
        Q1groupB5 = belgium5;
        Q1groupBC5 = belgiumC5;
        Q1groupBV5 = belgiumV5;
        Q1groupBD5 = belgiumD5;
        FQ1groupB = "Belgium";
    }

    else {}
    
    
    //2nd place results of group B
   
    //Columbia
    if (columbia > denmark && columbia > croatia && columbia < belgium) {
        cout << "Columbia is the second of Group B" << endl;
        Q2groupB = columbia;
        Q2groupBattack = columbiaattack;
        Q2groupBmidfield = columbiamidfield;
        Q2groupBdeffence = columbiadeffence;
        Q2groupBf = fcolumbia;
        Q2groupBcost = columbiacost;
        Q2groupBpop = columbiapop;
        Q2groupB5 = columbia5;
        Q2groupBC5 = columbiaC5;
        Q2groupBV5 = columbiaV5;
        Q2groupBD5 = columbiaD5;
        FQ2groupB = "Columbia";
    }

    else if (columbia > denmark && columbia < croatia && columbia > belgium) {
        cout << "Columbia is the second of Group B" << endl;
        Q2groupB = columbia;
        Q2groupBattack = columbiaattack;
        Q2groupBmidfield = columbiamidfield;
        Q2groupBdeffence = columbiadeffence;
        Q2groupBf = fcolumbia;
        Q2groupBcost = columbiacost;
        Q2groupBpop = columbiapop;
        Q2groupB5 = columbia5;
        Q2groupBC5 = columbiaC5;
        Q2groupBV5 = columbiaV5;
        Q2groupBD5 = columbiaD5;
        FQ2groupB = "Columbia";
    }

    else if (columbia < denmark && columbia > croatia && columbia > belgium) {
        cout << "Columbia is the second of Group B" << endl;
        Q2groupB = columbia;
        Q2groupBattack = columbiaattack;
        Q2groupBmidfield = columbiamidfield;
        Q2groupBdeffence = columbiadeffence;
        Q2groupBf = fcolumbia;
        Q2groupBcost = columbiacost;
        Q2groupBpop = columbiapop;
        Q2groupB5 = columbia5;
        Q2groupBC5 = columbiaC5;
        Q2groupBV5 = columbiaV5;
        Q2groupBD5 = columbiaD5;
        FQ2groupB = "Columbia";
    }

    else {}

    //Denmark
    if (denmark > columbia && denmark > croatia && denmark < belgium) {
        cout << "Denmark is the second of Group B" << endl;
        Q2groupB = denmark;
        Q2groupBattack = denmarkattack;
        Q2groupBmidfield = denmarkmidfield;
        Q2groupBdeffence = denmarkdeffence;
        Q2groupBf = fdenmark;
        Q2groupBcost = denmarkcost;
        Q2groupBpop = denmarkpop;
        Q2groupB5 = denmark5;
        Q2groupBC5 = denmarkC5;
        Q2groupBV5 = denmarkV5;
        Q2groupBD5 = denmarkD5;
        FQ2groupB = "Denmark";
    }

    else if (denmark > columbia && denmark < croatia && denmark > belgium) {
        cout << "Denmark is the second of Group B" << endl;
        Q2groupB = denmark;
        Q2groupBattack = denmarkattack;
        Q2groupBmidfield = denmarkmidfield;
        Q2groupBdeffence = denmarkdeffence;
        Q2groupBf = fdenmark;
        Q2groupBcost = denmarkcost;
        Q2groupBpop = denmarkpop;
        Q2groupB5 = denmark5;
        Q2groupBC5 = denmarkC5;
        Q2groupBV5 = denmarkV5;
        Q2groupBD5 = denmarkD5;
        FQ2groupB = "Denmark";
    }

    else if (denmark < columbia && denmark > croatia && denmark > belgium) {
        cout << "Denmark is the second of Group B" << endl;
        Q2groupB = denmark;
        Q2groupBattack = denmarkattack;
        Q2groupBmidfield = denmarkmidfield;
        Q2groupBdeffence = denmarkdeffence;
        Q2groupBf = fdenmark;
        Q2groupBcost = denmarkcost;
        Q2groupBpop = denmarkpop;
        Q2groupB5 = denmark5;
        Q2groupBC5 = denmarkC5;
        Q2groupBV5 = denmarkV5;
        Q2groupBD5 = denmarkD5;
        FQ2groupB = "Denmark";
    }

    else {}

    //Croatia
    if (croatia > denmark && croatia > belgium && croatia < columbia) {
        cout << "Croatia is the second of Group B" << endl;
        Q2groupB = croatia;
        Q2groupBattack = croatiaattack;
        Q2groupBmidfield = croatiamidfield;
        Q2groupBdeffence = croatiadeffence;
        Q2groupBf = fcroatia;
        Q2groupBcost = croatiacost;
        Q2groupBpop = croatiapop;
        Q2groupB5 = croatia5;
        Q2groupBC5 = croatiaC5;
        Q2groupBV5 = croatiaV5;
        Q2groupBD5 = croatiaD5;
        FQ2groupB = "Croatia";
    }

    else if (croatia > denmark && croatia < belgium && croatia > columbia) {
        cout << "Croatia is the second of Group B" << endl;
        Q2groupB = croatia;
        Q2groupBattack = croatiaattack;
        Q2groupBmidfield = croatiamidfield;
        Q2groupBdeffence = croatiadeffence;
        Q2groupBf = fcroatia;
        Q2groupBcost = croatiacost;
        Q2groupBpop = croatiapop;
        Q2groupB5 = croatia5;
        Q2groupBC5 = croatiaC5;
        Q2groupBV5 = croatiaV5;
        Q2groupBD5 = croatiaD5;
        FQ2groupB = "Croatia";
    }

    else if (croatia < denmark && croatia > belgium && croatia > columbia) {
        cout << "Croatia is the second of Group B" << endl;
        Q2groupB = croatia;
        Q2groupBattack = croatiaattack;
        Q2groupBmidfield = croatiamidfield;
        Q2groupBdeffence = croatiadeffence;
        Q2groupBf = fcroatia;
        Q2groupBcost = croatiacost;
        Q2groupBpop = croatiapop;
        Q2groupB5 = croatia5;
        Q2groupBC5 = croatiaC5;
        Q2groupBV5 = croatiaV5;
        Q2groupBD5 = croatiaD5;
        FQ2groupB = "Croatia";
    }

    else {}

    //Belgium
    if (belgium > denmark && belgium > croatia && belgium < columbia) {
        cout << "Belgium is the second of Group B" << endl;
        Q2groupB = belgium;
        Q2groupBattack = belgiumattack;
        Q2groupBmidfield = belgiummidfield;
        Q2groupBdeffence = belgiumdeffence;
        Q2groupBf = fbelgium;
        Q2groupBcost = belgiumcost;
        Q2groupBpop = belgiumpop;
        Q2groupB5 = belgium5;
        Q2groupBC5 = belgiumC5;
        Q2groupBV5 = belgiumV5;
        Q2groupBD5 = belgiumD5;
        FQ2groupB = "Belgium";
    }

    else if (belgium > denmark && belgium < croatia && belgium > columbia) {
        cout << "Belgium is  the second of Group B" << endl;
        Q2groupB = belgium;
        Q2groupBattack = belgiumattack;
        Q2groupBmidfield = belgiummidfield;
        Q2groupBdeffence = belgiumdeffence;
        Q2groupBf = fbelgium;
        Q2groupBcost = belgiumcost;
        Q2groupBpop = belgiumpop;
        Q2groupB5 = belgium5;
        Q2groupBC5 = belgiumC5;
        Q2groupBV5 = belgiumV5;
        Q2groupBD5 = belgiumD5;
        FQ2groupB = "Belgium";
    }

    else if (belgium < denmark && belgium > croatia && belgium > columbia) {
        cout << "Belgium is the second of Group B" << endl;
        Q2groupB = belgium;
        Q2groupBattack = belgiumattack;
        Q2groupBmidfield = belgiummidfield;
        Q2groupBdeffence = belgiumdeffence;
        Q2groupBf = fbelgium;
        Q2groupBcost = belgiumcost;
        Q2groupBpop = belgiumpop;
        Q2groupB5 = belgium5;
        Q2groupBC5 = belgiumC5;
        Q2groupBV5 = belgiumV5;
        Q2groupBD5 = belgiumD5;
        FQ2groupB = "Belgium";
    }

    else {}

    //There are many if statements for this because every team's individual statistic is competing with every team's individual statistic.

    //group A

    //attack of italy
    if (italyattack > portugalattack) {
        italy += 5;
    }
    
    if (italyattack > australiaattack) {
        italy += 5;
    }

    if (italyattack > iranattack) {
        italy += 5;
    }

    //attack of portugal
    if (portugalattack > italyattack) {
        portugal += 5;
    }

    if (portugalattack > australiaattack) {
        portugal += 5;
    }

    if (portugalattack > iranattack) {
        portugal += 5;
    }

    //attack of australia
    if (australiaattack > italyattack) {
        australia += 5;
    }

    if (australiaattack > portugalattack) {
        australia += 5;
    }

    if (australiaattack > iranattack) {
        australia += 5;
    }

    //attack of iran
    if (iranattack > italyattack) {
        iran += 5;
    }

    if (iranattack > portugalattack) {
        iran += 5;
    }

    if (iranattack > australiaattack) {
        iran += 5;
    }

    //midfield of italy
    if (italymidfield > portugalmidfield) {
        italy += 5;
    }
    
    if (italymidfield > australiamidfield) {
        italy += 5;
    }

    if (italymidfield > iranmidfield) {
        italy += 5;
    }

    //midfield of portugal
    if (portugalmidfield > italymidfield) {
        portugal += 5;
    }
    
    if (portugalmidfield > australiamidfield) {
        portugal += 5;
    }

    if (portugalmidfield > iranmidfield) {
        portugal += 5;
    }

    //midfield of australia
    if (australiamidfield > italymidfield) {
        australia += 5;
    }
    
    if (australiamidfield > portugalmidfield) {
        australia += 5;
    }

    if (australiamidfield > iranmidfield) {
        australia += 5;
    }

    //midfield of iran
    if (iranmidfield > italymidfield) {
        iran += 5;
    }
    
    if (iranmidfield > portugalmidfield) {
        iran += 5;
    }

    if (iranmidfield > australiamidfield) {
        iran += 5;
    }

    //deffence of italy
    if (italydeffence > portugaldeffence) {
        italy += 5;
    }
    
    if (italydeffence > australiadeffence) {
        italy += 5;
    }

    if (italydeffence > irandeffence) {
        italy += 5;
    }

    //deffence of portugal
    if (portugaldeffence > italydeffence) {
        portugal += 5;
    }
    
    if (portugaldeffence > australiadeffence) {
        portugal += 5;
    }

    if (portugaldeffence > irandeffence) {
        portugal += 5;
    }
    
    //deffence of australia
    if (australiadeffence > italydeffence) {
        australia += 5;
    }
    
    if (australiadeffence > portugaldeffence) {
        australia += 5;
    }

    if (australiadeffence > irandeffence) {
        australia += 5;
    }

    //deffence of iran
    if (irandeffence > italydeffence) {
        iran += 5;
    }
    
    if (irandeffence > portugaldeffence) {
        iran += 5;
    }

    if (irandeffence > australiadeffence) {
        iran += 5;
    }

    //cost of italy
    if (italycost > portugalcost) {
        italy += 3;
    }
    
    if (italycost > australiacost) {
        italy += 3;
    }

    if (italycost > irancost) {
        italy += 3;
    }

    //cost of portugal
    if (portugalcost > italycost) {
        portugal += 3;
    }
    
    if (portugalcost > australiacost) {
        portugal += 3;
    }

    if (portugalcost > irancost) {
        portugal += 3;
    }

    //cost of australia
    if (australiacost > italycost) {
        australia += 3;
    }
    
    if (australiacost > portugalcost) {
        australia += 3;
    }

    if (australiacost > irancost) {
        australia += 3;
    }

    //cost of iran
    if (irancost > italycost) {
        iran += 3;
    }
    
    if (irancost > portugalcost) {
        iran += 3;
    }

    if (irancost > australiacost) {
        iran += 3;
    }

    //population of iran
    if (iranpop > australiapop) {
        iran += 3;
    }
    
    if (iranpop > portugalpop) {
        iran += 3;
    }

    if (iranpop > italypop) {
        iran += 3;
    }

    //population of australia
    if (australiapop > iranpop) {
        australia += 3;
    }
    
    if (australiapop > portugalpop) {
        australia += 3;
    }

    if (australiapop > italypop) {
        australia += 3;
    }

    //population of portugal
    if (portugalpop > iranpop) {
        portugal += 3;
    }
    
    if (portugalpop > australiapop) {
        portugal += 3;
    }

    if (portugalpop > italypop) {
        portugal += 3;
    }

    //population of italy
    if (italypop > iranpop) {
        italy += 3;
    }
    
    if (italypop > australiapop) {
        italy += 3;
    }

    if (italypop > portugalpop) {
        italy += 3;
    }

    //italy # of goals score in last 5 games
    if (italy5 > portugal5) {
        italy += 1;
    }
    
    if (italy5 > australia5) {
        italy += 1;
    }

    if (italy5 > iran5) {
        italy += 1;
    }

    //portugal # of goals score in last 5 games
    if (portugal5 > italy5) {
        portugal += 1;
    }
    
    if (portugal5 > australia5) {
        portugal += 1;
    }

    if (portugal5 > iran5) {
        portugal += 1;
    }

    //australia # of goals score in last 5 games
    if (australia5 > italy5) {
        australia += 1;
    }
    
    if (australia5 > portugal5) {
        australia += 1;
    }

    if (australia5 > iran5) {
        australia += 1;
    }
    
    //iran # of goals score in last 5 games
    if (iran5 > italy5) {
        iran += 1;
    }
    
    if (iran5 > portugal5) {
        iran += 1;
    }

    if (iran5 > australia5) {
        iran += 1;
    }

    //iran # of goals conceded in last 5 games
    if (iranC5 > australiaC5) {
        iran -= 1;
    }
    
    if (iranC5 > portugalC5) {
        iran -= 1;
    }

    if (iranC5 > italyC5) {
        iran -= 1;
    }
    
    //australia # of goals conceded in last 5 games
    if (australiaC5 > iranC5) {
        australia -= 1;
    }
    
    if (australiaC5 > portugalC5) {
        australia -= 1;
    }

    if (australiaC5 > italyC5) {
        australia -= 1;
    }

    //portugal # of goals conceded in last 5 games
    if (portugalC5 > iranC5) {
        portugal -= 1;
    }
    
    if (portugalC5 > australiaC5) {
        portugal -= 1;
    }

    if (portugalC5 > italyC5) {
        portugal -= 1;
    }

    //italy # of goals conceded in last 5 games
    if (italyC5 > iranC5) {
        italy -= 1;
    }
    
    if (italyC5 > australiaC5) {
        italy -= 1;
    }

    if (italyC5 > portugalC5) {
        italy -= 1;
    }

    //italy # of goals victory in last 5 games
    if (italyV5 > portugalV5) {
        italy += 1;
    }
    
    if (italyV5 > australiaV5) {
        italy += 1;
    }

    if (italyV5 > iranV5) {
        italy += 1;
    }

    //portugal # of goals victory in last 5 games
    if (portugalV5 > italyV5) {
        portugal += 1;
    }
    
    if (portugalV5 > australiaV5) {
        portugal += 1;
    }

    if (portugalV5 > iranV5) {
        portugal += 1;
    }

    //australia # of goals victory in last 5 games
    if (australiaV5 > italyV5) {
        australia += 1;
    }
    
    if (australiaV5 > portugalV5) {
        australia += 1;
    }

    if (australiaV5 > iranV5) {
        australia += 1;
    }

    //iran # of goals victory in last 5 games
    if (iranV5 > italyV5) {
        iran += 1;
    }
    
    if (iranV5 > portugalV5) {
        iran += 1;
    }

    if (iranV5 > australiaV5) {
        iran += 1;
    }

    //iran # of defeats in last 5 games
    if (iranD5 > australiaD5) {
        iran -= 1;
    }
    
    if (iranD5 > portugalD5) {
        iran -= 1;
    }

    if (iranD5 > italyD5) {
        iran -= 1;
    }

    //australia # of defeats in last 5 games
    if (australiaD5 > iranD5) {
        australia -= 1;
    }
    
    if (australiaD5 > portugalD5) {
        australia -= 1;
    }

    if (australiaD5 > italyD5) {
        australia -= 1;
    }

    //portugal # of defeats in last 5 games
    if (portugalD5 > iranD5) {
        portugal -= 1;
    }
    
    if (portugalD5 > australiaD5) {
        portugal -= 1;
    }

    if (portugalD5 > italyD5) {
        portugal -= 1;
    }

    //italy # of defeats in last 5 games
    if (italyD5 > iranD5) {
        italy -= 1;
    }
    
    if (italyD5 > australiaD5) {
        italy -= 1;
    }

    if (italyD5 > portugalD5) {
        italy -= 1;
    }

    //italy factor of unexpectancy
    if (fitaly > firan) {
        italy = italy + r29;
    }
    
    if (fitaly > faustralia) {
        italy = italy + r29;
    }

    if (fitaly > fportugal) {
        italy = italy + r29;
    }

    //iran factor of unexpectancy
    if (firan > fitaly) {
        iran = iran + r30;
    }
    
    if (firan > faustralia) {
        iran = iran + r30;
    }

    if (firan > fportugal) {
        iran = iran + r30;
    }

    //australia factor of unexpectancy
    if (faustralia > fitaly) {
        australia = australia + r31;
    }
    
    if (faustralia > firan) {
        australia = australia + r31;
    }

    if (faustralia > fportugal) {
        australia = australia + r31;
    }

    //portugal factor of unexpectancy
    if (fportugal > fitaly) {
        portugal = portugal + r32;
    }
    
    if (fportugal > firan) {
        portugal = portugal + r32;
    }

    if (fportugal > faustralia) {
        portugal = portugal + r32;
    }

    //1st place results
    if (italy > portugal && italy > australia && italy > iran) {
        cout << "Italy is the winner of Group A" << endl;
        Q1groupA = italy;
        Q1groupAattack = italyattack;
        Q1groupAmidfield = italymidfield;
        Q1groupAdeffence = italydeffence;
        Q1groupAf = fitaly;
        Q1groupAcost = italycost;
        Q1groupApop = italypop;
        Q1groupA5 = italy5;
        Q1groupAC5 = italyC5;
        Q1groupAV5 = italyV5;
        Q1groupAD5 = italyD5;
        FQ1groupA = "Italy";
    }

    else if (portugal > italy && portugal > australia && portugal > iran) {
        cout << "Portugal is the winner of Group A" << endl;
        Q1groupA = portugal;
        Q1groupAattack = portugalattack;
        Q1groupAmidfield = portugalmidfield;
        Q1groupAdeffence = portugaldeffence;
        Q1groupAf = fportugal;
        Q1groupAcost = portugalcost;
        Q1groupApop = portugalpop;
        Q1groupA5 = portugal5;
        Q1groupAC5 = portugalC5;
        Q1groupAV5 = portugalV5;
        Q1groupAD5 = portugalD5;
        FQ1groupA = "Portugal";
    }

    else if (australia > italy && australia > portugal && australia > iran) {
        cout << "Australia is the winner of Group A" << endl;
        Q1groupA = australia;
        Q1groupAattack = australiaattack;
        Q1groupAmidfield = australiamidfield;
        Q1groupAdeffence = australiadeffence;
        Q1groupAf = faustralia;
        Q1groupAcost = australiacost;
        Q1groupApop = australiapop;
        Q1groupA5 = australia5;
        Q1groupAC5 = australiaC5;
        Q1groupAV5 = australiaV5;
        Q1groupAD5 = australiaD5;
        FQ1groupA = "Australia";
    }

    else if (iran > italy && iran > portugal && iran > australia) {
        cout << "Iran is the winner of Group A" << endl;
        Q1groupA = iran;
        Q1groupAattack = iranattack;
        Q1groupAmidfield = iranmidfield;
        Q1groupAdeffence = irandeffence;
        Q1groupAf = firan;
        Q1groupAcost = irancost;
        Q1groupApop = iranpop;
        Q1groupA5 = iran5;
        Q1groupAC5 = iranC5;
        Q1groupAV5 = iranV5;
        Q1groupAD5 = iranD5;
        FQ1groupA = "Iran";
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
        Q2groupAf = fitaly;
        Q2groupAcost = italycost;
        Q2groupApop = italypop;
        Q2groupA5 = italy5;
        Q2groupAC5 = italyC5;
        Q2groupAV5 = italyV5;
        Q2groupAD5 = italyD5;
        FQ2groupA = "Italy";
    }

    else if (italy > portugal && italy < australia && italy > iran) {
        cout << "Italy is the second of Group A" << endl;
        Q2groupA = italy;
        Q2groupAattack = italyattack;
        Q2groupAmidfield = italymidfield;
        Q2groupAdeffence = italydeffence;
        Q2groupAf = fitaly;
        Q2groupAcost = italycost;
        Q2groupApop = italypop;
        Q2groupA5 = italy5;
        Q2groupAC5 = italyC5;
        Q2groupAV5 = italyV5;
        Q2groupAD5 = italyD5;
        FQ2groupA = "Italy";
    }

    else if (italy < portugal && italy > australia && italy > iran) {
        cout << "Italy is the second of Group A" << endl;
        Q2groupA = italy;
        Q2groupAattack = italyattack;
        Q2groupAmidfield = italymidfield;
        Q2groupAdeffence = italydeffence;
        Q2groupAf = fitaly;
        Q2groupAcost = italycost;
        Q2groupApop = italypop;
        Q2groupA5 = italy5;
        Q2groupAC5 = italyC5;
        Q2groupAV5 = italyV5;
        Q2groupAD5 = italyD5;
        FQ2groupA = "Italy";
    }

    else {}

    //Portugal
    if (portugal > italy && portugal > australia && portugal < iran) {
        cout << "Portugal is the second of Group A" << endl;
        Q2groupA = portugal;
        Q2groupAattack = portugalattack;
        Q2groupAmidfield = portugalmidfield;
        Q2groupAdeffence = portugaldeffence;
        Q1groupAf = fportugal;
        Q1groupAcost = portugalcost;
        Q1groupApop = portugalpop;
        Q1groupA5 = portugal5;
        Q1groupAC5 = portugalC5;
        Q1groupAV5 = portugalV5;
        Q1groupAD5 = portugalD5;
        FQ2groupA = "Portugal";
    }

    else if (portugal > italy && portugal < australia && portugal > iran) {
        cout << "Portugal is the second of Group A" << endl;
        Q2groupA = portugal;
        Q2groupAattack = portugalattack;
        Q2groupAmidfield = portugalmidfield;
        Q2groupAdeffence = portugaldeffence;
        Q1groupAf = fportugal;
        Q1groupAcost = portugalcost;
        Q1groupApop = portugalpop;
        Q1groupA5 = portugal5;
        Q1groupAC5 = portugalC5;
        Q1groupAV5 = portugalV5;
        Q1groupAD5 = portugalD5;
        FQ2groupA = "Portugal";
    }

    else if (portugal < italy && portugal > australia && portugal > iran) {
        cout << "Portugal is the second of Group A" << endl;
        Q2groupA = portugal;
        Q2groupAattack = portugalattack;
        Q2groupAmidfield = portugalmidfield;
        Q2groupAdeffence = portugaldeffence;
        Q1groupAf = fportugal;
        Q1groupAcost = portugalcost;
        Q1groupApop = portugalpop;
        Q1groupA5 = portugal5;
        Q1groupAC5 = portugalC5;
        Q1groupAV5 = portugalV5;
        Q1groupAD5 = portugalD5;
        FQ2groupA = "Portugal";
    }

    else {}

    //Australia
    if (australia > italy && australia > portugal && australia < iran) {
        cout << "Australia is the second of Group A" << endl;
        Q2groupA = australia;
        Q2groupAattack = australiaattack;
        Q2groupAmidfield = australiamidfield;
        Q2groupAdeffence = australiadeffence;
        Q1groupAf = faustralia;
        Q1groupAcost = australiacost;
        Q1groupApop = australiapop;
        Q1groupA5 = australia5;
        Q1groupAC5 = australiaC5;
        Q1groupAV5 = australiaV5;
        Q1groupAD5 = australiaD5;
        FQ2groupA = "Australia";
    }

    else if (australia > italy && australia < portugal && australia > iran) {
        cout << "Australia is the second of Group A" << endl;
        Q2groupA = australia;
        Q2groupAattack = australiaattack;
        Q2groupAmidfield = australiamidfield;
        Q2groupAdeffence = australiadeffence;
        Q1groupAf = faustralia;
        Q1groupAcost = australiacost;
        Q1groupApop = australiapop;
        Q1groupA5 = australia5;
        Q1groupAC5 = australiaC5;
        Q1groupAV5 = australiaV5;
        Q1groupAD5 = australiaD5;
        FQ2groupA = "Australia";
    }

    else if (australia < italy && australia > portugal && australia > iran) {
        cout << "Australia is the second of Group A" << endl;
        Q2groupA = australia;
        Q2groupAattack = australiaattack;
        Q2groupAmidfield = australiamidfield;
        Q2groupAdeffence = australiadeffence;
        Q1groupAf = faustralia;
        Q1groupAcost = australiacost;
        Q1groupApop = australiapop;
        Q1groupA5 = australia5;
        Q1groupAC5 = australiaC5;
        Q1groupAV5 = australiaV5;
        Q1groupAD5 = australiaD5;
        FQ2groupA = "Australia";
    }

    else {}

    //Iran
    if (iran > italy && iran > portugal && iran < australia) {
        cout << "Iran is the second of Group A" << endl;
        Q2groupA = iran;
        Q2groupAattack = iranattack;
        Q2groupAmidfield = iranmidfield;
        Q2groupAdeffence = irandeffence;
        Q1groupAf = firan;
        Q1groupAcost = irancost;
        Q1groupApop = iranpop;
        Q1groupA5 = iran5;
        Q1groupAC5 = iranC5;
        Q1groupAV5 = iranV5;
        Q1groupAD5 = iranD5;
        FQ2groupA = "Iran";
    }

    else if (iran > italy && iran < portugal && iran > australia) {
        cout << "Iran is the second of Group A" << endl;
        Q2groupA = iran;
        Q2groupAattack = iranattack;
        Q2groupAmidfield = iranmidfield;
        Q2groupAdeffence = irandeffence;
        Q1groupAf = firan;
        Q1groupAcost = irancost;
        Q1groupApop = iranpop;
        Q1groupA5 = iran5;
        Q1groupAC5 = iranC5;
        Q1groupAV5 = iranV5;
        Q1groupAD5 = iranD5;
        FQ2groupA = "Iran";
    }

    else if (iran < italy && iran > portugal && iran > australia) {
        cout << "Iran is the second of Group A" << endl;
        Q2groupA = iran;
        Q2groupAattack = iranattack;
        Q2groupAmidfield = iranmidfield;
        Q2groupAdeffence = irandeffence;
        Q1groupAf = firan;
        Q1groupAcost = irancost;
        Q1groupApop = iranpop;
        Q1groupA5 = iran5;
        Q1groupAC5 = iranC5;
        Q1groupAV5 = iranV5;
        Q1groupAD5 = iranD5;
        FQ2groupA = "Iran";
    }

    else {}
    

    //Qualification matches

    //Now, we're competing against the teams who are the winners in their specific groups. The following comparsion is between the winners of the group to decide which team is going to qualify for quarter finals
    
    //Qualified teams' attack, midfield, deffence difference
    
    //Game one's comparison

    //Attack
    if (Q1groupAattack > Q2groupBattack) {
        Q1groupA += 6;
    }

    else if (Q1groupAattack < Q2groupBattack) {
        Q2groupB += 6;
    }

    //midfield
    if (Q1groupAmidfield > Q2groupBmidfield) {
        Q1groupA += 6;
    }

    else if (Q1groupAmidfield < Q2groupBmidfield) {
        Q2groupB += 6;
    }

    //deffence
    if (Q1groupAdeffence > Q2groupBdeffence) {
        Q1groupA += 6;
    }

    else if (Q1groupAdeffence < Q2groupBdeffence) {
        Q2groupB += 6;
    }
    
    //factor of unexpectancy
    if (Q1groupAf > Q2groupBf) {
        Q1groupA += 4;
    }

    else if (Q1groupAf < Q2groupBf) {
        Q2groupB += 4;
    }
    //cost of teams
    if (Q1groupAcost > Q2groupBcost) {
        Q1groupA += 4;
    }

    else if (Q1groupAcost < Q2groupBcost) {
        Q2groupB += 4;
    }
    //popuplation
    if (Q1groupApop > Q2groupBpop) {
        Q1groupA += 4;
    }

    else if (Q1groupApop < Q2groupBpop) {
        Q2groupB += 4;
    }
    
    //# of goals score in last 5 games
    if (Q1groupA5 > Q2groupB5) {
        Q1groupA += 1;
    }

    else if (Q1groupA5 < Q2groupB5) {
        Q2groupB += 1;
    }

    //# of goals conceded in last 5 games
    if (Q1groupAC5 > Q2groupBC5) {
        Q1groupA -= 1;
    }

    else if (Q1groupAC5 < Q2groupBC5) {
        Q2groupB -= 1;
    }

    //# of victories in last 5 games
    if (Q1groupAV5 > Q2groupBV5) {
        Q1groupA += 1;
    }

    else if (Q1groupAV5 < Q2groupBV5) {
        Q2groupB += 1;
    }
    //# of defeats in last 5 games
    if (Q1groupAD5 > Q2groupBD5) {
        Q1groupA -= 1;
    }

    else if (Q1groupAD5 < Q2groupBD5) {
        Q2groupB -= 1;
    }
    
    //Game two's comparison

    //Attack
    if (Q1groupBattack > Q2groupAattack) {
        Q1groupB += 6;
    }

    else if (Q1groupBattack < Q2groupAattack) {
        Q2groupA += 6;
    }

    //midfield
    if (Q1groupBmidfield > Q2groupAmidfield) {
        Q1groupB += 6;
    }

    else if (Q1groupBmidfield < Q2groupAmidfield) {
        Q2groupA += 6;
    }

    //deffence
    if (Q1groupBdeffence > Q2groupAdeffence) {
        Q1groupB += 6;
    }

    else if (Q1groupBdeffence < Q2groupAdeffence) {
        Q2groupA += 6;
    }
    
    
    //factor of unexpectancy
    if (Q1groupBf > Q2groupAf) {
        Q1groupB += 4;
    }

    else if (Q1groupBf < Q2groupAf) {
        Q2groupA += 4;
    }
    //cost of teams
    if (Q1groupBcost > Q2groupAcost) {
        Q1groupB += 4;
    }

    else if (Q1groupBcost < Q2groupAcost) {
        Q2groupA += 4;
    }
    //popuplation
    if (Q1groupBpop > Q2groupApop) {
        Q1groupB += 4;
    }

    else if (Q1groupBpop < Q2groupApop) {
        Q2groupA += 4;
    }
    
    //# of goals score in last 5 games
    if (Q1groupB5 > Q2groupA5) {
        Q1groupB += 1;
    }

    else if (Q1groupB5 < Q2groupA5) {
        Q2groupA += 1;
    }
    //# of goals conceded in last 5 games
    if (Q1groupBC5 > Q2groupAC5) {
        Q1groupB -= 1;
    }

    else if (Q1groupBC5 < Q2groupAC5) {
        Q2groupA -= 1;
    }
    //# of victories in last 5 games
    if (Q1groupBV5 > Q2groupAV5) {
        Q1groupB += 1;
    }

    else if (Q1groupBV5 < Q2groupAV5) {
        Q2groupA += 1;
    }
    //# of defeats in last 5 games
    if (Q1groupBD5 > Q2groupAD5) {
        Q1groupB -= 1;
    }

    else if (Q1groupBD5 < Q2groupAD5) {
        Q2groupA -= 1;
    }

    
    
    //Game three's comparison

    //Attack
    if (Q1groupCattack > Q2groupDattack) {
        Q1groupC += 6;
    }

    else if (Q1groupCattack < Q2groupDattack) {
        Q2groupD += 6;
    }

    //midfield
    if (Q1groupCmidfield > Q2groupDmidfield) {
        Q1groupC += 6;
    }

    else if (Q1groupCmidfield < Q2groupDmidfield) {
        Q2groupD += 6;
    }

    //deffence
    if (Q1groupCdeffence > Q2groupDdeffence) {
        Q1groupC += 6;
    }

    else if (Q1groupCdeffence < Q2groupDdeffence) {
        Q2groupD += 6;
    }
    
    
    //factor of unexpectancy
    if (Q1groupCf > Q2groupDf) {
        Q1groupC += 4;
    }

    else if (Q1groupCf < Q2groupDf) {
        Q2groupD += 4;
    }
    //cost of teams
    if (Q1groupCcost > Q2groupDcost) {
        Q1groupC += 4;
    }

    else if (Q1groupCcost < Q2groupDcost) {
        Q2groupD += 4;
    }
    //popuplation
    if (Q1groupCpop > Q2groupDpop) {
        Q1groupC += 4;
    }

    else if (Q1groupCpop < Q2groupDpop) {
        Q2groupD += 4;
    }
    
    //# of goals score in last 5 games
    if (Q1groupC5 > Q2groupD5) {
        Q1groupC += 1;
    }

    else if (Q1groupC5 < Q2groupD5) {
        Q2groupD += 1;
    }

    //# of goals conceded in last 5 games
    if (Q1groupCC5 > Q2groupDC5) {
        Q1groupC -= 1;
    }

    else if (Q1groupCC5 < Q2groupDC5) {
        Q2groupD -= 1;
    }

    //# of victories in last 5 games
    if (Q1groupCV5 > Q2groupDV5) {
        Q1groupC += 1;
    }

    else if (Q1groupCV5 < Q2groupDV5) {
        Q2groupD += 1;
    }
    //# of defeats in last 5 games
    if (Q1groupCD5 > Q2groupDD5) {
        Q1groupC -= 1;
    }

    else if (Q1groupCD5 < Q2groupDD5) {
        Q2groupD -= 1;
    }


    //Game four's comparison

    //Attack
    if (Q2groupCattack > Q1groupDattack) {
        Q2groupC += 6;
    }

    else if (Q2groupCattack < Q1groupDattack) {
        Q1groupD += 6;
    }

    //midfield
    if (Q2groupCmidfield > Q1groupDmidfield) {
        Q2groupC += 6;
    }

    else if (Q2groupCmidfield < Q1groupDmidfield) {
        Q1groupD += 6;
    }

    //deffence
    if (Q2groupCdeffence > Q1groupDdeffence) {
        Q2groupC += 6;
    }

    else if (Q2groupCdeffence < Q1groupDdeffence) {
        Q1groupD += 6;
    }
    
    //factor of unexpectancy
    if (Q2groupCf > Q1groupDf) {
        Q2groupC += 4;
    }

    else if (Q2groupCf < Q1groupDf) {
        Q1groupD += 4;
    }
    //cost of teams
    if (Q2groupCcost > Q1groupDcost) {
        Q2groupC += 4;
    }

    else if (Q2groupCcost < Q1groupDcost) {
        Q1groupD += 4;
    }
    //popuplation
    if (Q2groupCpop > Q1groupDpop) {
        Q2groupC += 4;
    }

    else if (Q2groupCpop < Q1groupDpop) {
        Q1groupD += 4;
    }
    
    //# of goals score in last 5 games
    if (Q2groupC5 > Q1groupD5) {
        Q2groupC += 1;
    }

    else if (Q2groupC5 < Q1groupD5) {
        Q1groupD += 1;
    }

    //# of goals conceded in last 5 games
    if (Q2groupCC5 > Q1groupDC5) {
        Q2groupC -= 1;
    }

    else if (Q2groupCC5 < Q1groupDC5) {
        Q1groupD -= 1;
    }

    //# of victories in last 5 games
    if (Q2groupCV5 > Q1groupDV5) {
        Q2groupC += 1;
    }

    else if (Q2groupCV5 < Q1groupDV5) {
        Q1groupD += 1;
    }
    //# of defeats in last 5 games
    if (Q2groupCD5 > Q1groupDD5) {
        Q2groupC -= 1;
    }

    else if (Q2groupCD5 < Q1groupDD5) {
        Q1groupD -= 1;
    }

    //Game five's comparison

    //Attack
    if (Q1groupEattack > Q2groupFattack) {
        Q1groupE += 6;
    }

    else if (Q1groupEattack < Q2groupFattack) {
        Q2groupF += 6;
    }

    //midfield
    if (Q1groupEmidfield > Q2groupFmidfield) {
        Q1groupE += 6;
    }

    else if (Q1groupEmidfield < Q2groupFmidfield) {
        Q2groupF += 6;
    }

    //defense
    if (Q1groupEdeffence > Q2groupFdeffence) {
        Q1groupE += 6;
    }

    else if (Q1groupEdeffence < Q2groupFdeffence) {
        Q2groupF += 6;
    }
    
    //factor of unexpectancy
    if (Q1groupEf > Q2groupFf) {
        Q1groupE += 4;
    }

    else if (Q1groupEf < Q2groupFf) {
        Q2groupF += 4;
    }
    //cost of teams
    if (Q1groupEcost > Q2groupFcost) {
        Q1groupE += 4;
    }

    else if (Q1groupEcost < Q2groupFcost) {
        Q2groupF += 4;
    }
    //popuplation
    if (Q1groupEpop > Q2groupFpop) {
        Q1groupE += 4;
    }

    else if (Q1groupEpop < Q2groupFpop) {
        Q2groupF += 4;
    }
    
    //# of goals score in last 5 games
    if (Q1groupE5 > Q2groupF5) {
        Q1groupE += 1;
    }

    else if (Q1groupE5 < Q2groupF5) {
        Q2groupF += 1;
    }

    //# of goals conceded in last 5 games
    if (Q1groupEC5 > Q2groupFC5) {
        Q1groupE -= 1;
    }

    else if (Q1groupEC5 < Q2groupFC5) {
        Q2groupF -= 1;
    }

    //# of victories in last 5 games
    if (Q1groupEV5 > Q2groupFV5) {
        Q1groupE += 1;
    }

    else if (Q1groupEV5 < Q2groupFV5) {
        Q2groupF += 1;
    }
    //# of defeats in last 5 games
    if (Q1groupED5 > Q2groupFD5) {
        Q1groupE -= 1;
    }

    else if (Q1groupED5 < Q2groupFD5) {
        Q2groupF -= 1;
    }

    //Game six's comparison

    //Attack
    if (Q2groupEattack > Q1groupFattack) {
        Q2groupE += 6;
    }

    else if (Q2groupEattack < Q1groupFattack) {
        Q1groupF += 6;
    }

    //midfield
    if (Q2groupEmidfield > Q1groupFmidfield) {
        Q2groupE += 6;
    }

    else if (Q2groupEmidfield < Q1groupFmidfield) {
        Q1groupF += 6;
    }

    //defense
    if (Q2groupEdeffence > Q1groupFdeffence) {
        Q2groupE += 6;
    }

    else if (Q2groupEdeffence < Q1groupFdeffence) {
        Q1groupF += 6;
    }
    
    //factor of unexpectancy
    if (Q2groupEf > Q1groupFf) {
        Q2groupE += 4;
    }

    else if (Q2groupEf < Q1groupFf) {
        Q1groupF += 4;
    }
    //cost of teams
    if (Q2groupEcost > Q1groupFcost) {
        Q2groupE += 4;
    }

    else if (Q2groupEcost < Q1groupFcost) {
        Q1groupF += 4;
    }
    //population
    if (Q2groupEpop > Q1groupFpop) {
        Q2groupE += 4;
    }

    else if (Q2groupEpop < Q1groupFpop) {
        Q2groupF += 4;
    }
    
    //# of goals score in last 5 games
    if (Q2groupE5 > Q1groupF5) {
        Q2groupE += 1;
    }

    else if (Q2groupE5 < Q1groupF5) {
        Q1groupF += 1;
    }

    //# of goals conceded in last 5 games
    if (Q2groupEC5 > Q1groupFC5) {
        Q2groupE -= 1;
    }

    else if (Q2groupEC5 < Q1groupFC5) {
        Q1groupF -= 1;
    }

    //# of victories in last 5 games
    if (Q2groupEV5 > Q1groupFV5) {
        Q2groupE += 1;
    }

    else if (Q2groupEV5 < Q1groupFV5) {
        Q1groupF += 1;
    }
    //# of defeats in last 5 games
    if (Q2groupED5 > Q1groupFD5) {
        Q2groupE -= 1;
    }

    else if (Q2groupED5 < Q1groupFD5) {
        Q1groupF -= 1;
    }


    //Game seven's comparison

    //Attack
    if (Q1groupGattack > Q2groupHattack) {
        Q1groupG += 6;
    }

    else if (Q1groupGattack < Q2groupHattack) {
        Q2groupH += 6;
    }

    //midfield
    if (Q1groupGmidfield > Q2groupHmidfield) {
        Q1groupG += 6;
    }

    else if (Q1groupGmidfield < Q2groupHmidfield) {
        Q2groupH += 6;
    }

    //deffence
    if (Q1groupGdeffence > Q2groupHdeffence) {
        Q1groupG += 6;
    }

    else if (Q1groupGdeffence < Q2groupHdeffence) {
        Q2groupH += 6;
    }
    
    //factor of unexpectancy
    if (Q1groupGf > Q2groupHf) {
        Q1groupG += 4;
    }

    else if (Q1groupGf < Q2groupHf) {
        Q2groupH += 4;
    }
    //cost of teams
    if (Q1groupGcost > Q2groupHcost) {
        Q1groupG += 4;
    }

    else if (Q1groupGcost < Q2groupHcost) {
        Q2groupH += 4;
    }
    //popuplation
    if (Q1groupGpop > Q2groupHpop) {
        Q1groupG += 4;
    }

    else if (Q1groupGpop < Q2groupHpop) {
        Q2groupH += 4;
    }
    
    //# of goals score in last 5 games
    if (Q1groupG5 > Q2groupH5) {
        Q1groupG += 1;
    }

    else if (Q1groupG5 < Q2groupH5) {
        Q2groupH += 1;
    }

    //# of goals conceded in last 5 games
    if (Q1groupGC5 > Q2groupHC5) {
        Q1groupG -= 1;
    }

    else if (Q1groupGC5 < Q2groupHC5) {
        Q2groupH -= 1;
    }

    //# of victories in last 5 games
    if (Q1groupGV5 > Q2groupHV5) {
        Q1groupG += 1;
    }

    else if (Q1groupGV5 < Q2groupHV5) {
        Q2groupH += 1;
    }
    //# of defeats in last 5 games
    if (Q1groupGD5 > Q2groupHD5) {
        Q1groupG -= 1;
    }

    else if (Q1groupGD5 < Q2groupHD5) {
        Q2groupH -= 1;
    }


    //Game eight's comparison
    //Attack
    if (Q2groupGattack > Q1groupHattack) {
        Q2groupG += 6;
    }

    else if (Q2groupGattack < Q1groupHattack) {
        Q1groupH += 6;
    }

    //midfield
    if (Q2groupGmidfield > Q1groupHmidfield) {
        Q2groupG += 6;
    }

    else if (Q2groupGmidfield < Q1groupHmidfield) {
        Q1groupH += 6;
    }

    //deffence
    if (Q2groupGdeffence > Q1groupHdeffence) {
        Q2groupG += 6;
    }

    else if (Q2groupGdeffence < Q1groupHdeffence) {
        Q1groupH += 6;
    }
    
    
    //factor of unexpectancy
    if (Q2groupGf > Q1groupHf) {
        Q2groupG += 4;
    }

    else if (Q2groupGf < Q1groupHf) {
        Q1groupH += 4;
    }
    //cost of teams
    if (Q2groupGcost > Q1groupHcost) {
        Q2groupG += 4;
    }

    else if (Q2groupGcost < Q1groupHcost) {
        Q1groupH += 4;
    }
    //popuplation
    if (Q2groupGpop > Q1groupHpop) {
        Q2groupG += 4;
    }

    else if (Q2groupGpop < Q1groupHpop) {
        Q1groupH += 4;
    }
    
    //# of goals score in last 5 games
    if (Q2groupG5 > Q1groupH5) {
        Q2groupG += 1;
    }

    else if (Q2groupG5 < Q1groupH5) {
        Q1groupH += 1;
    }

    //# of goals conceded in last 5 games
    if (Q2groupGC5 > Q1groupHC5) {
        Q2groupG -= 1;
    }

    else if (Q2groupGC5 < Q1groupHC5) {
        Q1groupH -= 1;
    }

    //# of victories in last 5 games
    if (Q2groupGV5 > Q1groupHV5) {
        Q2groupG += 1;
    }

    else if (Q2groupGV5 < Q1groupHV5) {
        Q1groupH += 1;
    }
    //# of defeats in last 5 games
    if (Q2groupGD5 > Q1groupHD5) {
        Q2groupG -= 1;
    }

    else if (Q2groupGD5 < Q1groupHD5) {
        Q1groupH -= 1;
    }

    cout << endl;
     

    //The follwing code simulates and makes the compiler decide which team wins. It decided which game is won by whom

    //Round 1 match results
    //game 1
    if (Q1groupA > Q2groupB) {
        cout << FQ1groupA <<" won "<< FQ2groupB << " in round 1" << endl;
        QFgame1 = Q1groupA;
        QFgame1attack = Q1groupAattack;
        QFgame1midfield = Q1groupAmidfield;
        QFgame1deffence = Q1groupAdeffence;
        QFgame1f = Q1groupAf;
        QFgame1cost = Q1groupAcost;
        QFgame1pop = Q1groupApop;
        QFgame15 = Q1groupA5;
        QFgame1C5 = Q1groupAC5;
        QFgame1V5 = Q1groupAV5;
        QFgame1D5 = Q1groupAD5;
        
        FQFgame1 = FQ1groupA;
        
    }

    if (Q1groupA < Q2groupB) {
        cout << FQ2groupB <<" won "<< FQ1groupA << " in round 1" << endl;
        QFgame1 = Q2groupB;
        QFgame1attack = Q2groupBattack;
        QFgame1midfield = Q2groupBmidfield;
        QFgame1deffence = Q2groupBdeffence;
        QFgame1f = Q2groupBf;
        QFgame1cost = Q2groupBcost;
        QFgame1pop = Q2groupBpop;
        QFgame15 = Q2groupB5;
        QFgame1C5 = Q2groupBC5;
        QFgame1V5 = Q2groupBV5;
        QFgame1D5 = Q2groupBD5;
        
        FQFgame1 = FQ2groupB;
        
    }

    //game 2
    if (Q2groupA > Q1groupB) {
        cout << FQ2groupA <<" won "<< FQ1groupB << " in round 1" << endl;
        QFgame2 = Q2groupA;
        QFgame2attack = Q2groupAattack;
        QFgame2midfield = Q2groupAmidfield;
        QFgame2deffence = Q2groupAdeffence;
        QFgame2f = Q2groupAf;
        QFgame2cost = Q2groupAcost;
        QFgame2pop = Q2groupApop;
        QFgame25 = Q2groupA5;
        QFgame2C5 = Q2groupAC5;
        QFgame2V5 = Q2groupAV5;
        QFgame2D5 = Q2groupAD5;
       
        FQFgame2 = FQ2groupA;
        
    }

    if (Q2groupA < Q1groupB) {
        cout << FQ1groupB <<" won "<< FQ2groupA << " in round 1" << endl;
        QFgame2 = Q1groupB;
        QFgame2attack = Q1groupBattack;
        QFgame2midfield = Q1groupBmidfield;
        QFgame2deffence = Q1groupBdeffence;
        QFgame2f = Q1groupBf;
        QFgame2cost = Q1groupBcost;
        QFgame2pop = Q1groupBpop;
        QFgame25 = Q1groupB5;
        QFgame2C5 = Q1groupBC5;
        QFgame2V5 = Q1groupBV5;
        QFgame2D5 = Q1groupBD5;
        
        FQFgame2 = FQ1groupB;
        
    }

    //game 3
    if (Q1groupC > Q2groupD) {
        cout << FQ1groupC <<" won "<< FQ2groupD << " in round 1" << endl;
        QFgame3 = Q1groupC;
        QFgame3attack = Q1groupCattack;
        QFgame3midfield = Q1groupCmidfield;
        QFgame3deffence = Q1groupCdeffence;
        QFgame3f = Q1groupCf;
        QFgame3cost = Q1groupCcost;
        QFgame3pop = Q1groupCpop;
        QFgame35 = Q1groupC5;
        QFgame3C5 = Q1groupCC5;
        QFgame3V5 = Q1groupCV5;
        QFgame3D5 = Q1groupCD5;
        
        FQFgame3 = FQ1groupC;
        
    }

    if (Q1groupC < Q2groupD) {
        cout << FQ2groupD <<" won "<< FQ1groupC << " in round 1" << endl;
        QFgame3 = Q2groupD;
        QFgame3attack = Q2groupDattack;
        QFgame3midfield = Q2groupDmidfield;
        QFgame3deffence = Q2groupDdeffence;
        QFgame3f = Q2groupDf;
        QFgame3cost = Q2groupDcost;
        QFgame3pop = Q2groupDpop;
        QFgame35 = Q2groupD5;
        QFgame3C5 = Q2groupDC5;
        QFgame3V5 = Q2groupDV5;
        QFgame3D5 = Q2groupDD5;
        
        FQFgame3 = FQ2groupD;
        
    }

    //game 4
    if (Q2groupC > Q1groupD) {
        cout << FQ2groupC <<" won "<< FQ1groupD << " in round 1" << endl;
        QFgame4 = Q2groupC;
        QFgame4attack = Q2groupCattack;
        QFgame4midfield = Q2groupCmidfield;
        QFgame4deffence = Q2groupCdeffence;
        QFgame4f = Q2groupCf;
        QFgame4cost = Q2groupCcost;
        QFgame4pop = Q2groupCpop;
        QFgame45 = Q2groupC5;
        QFgame4C5 = Q2groupCC5;
        QFgame4V5 = Q2groupCV5;
        QFgame4D5 = Q2groupCD5;
        
        FQFgame4 = FQ2groupC;
        
    }

    if (Q2groupC < Q1groupD) {
        cout << FQ1groupD <<" won "<< FQ2groupC << " in round 1" << endl;
        QFgame4 = Q1groupD;
        QFgame4attack = Q1groupDattack;
        QFgame4midfield = Q1groupDmidfield;
        QFgame4deffence = Q1groupDdeffence;
        QFgame4f = Q1groupDf;
        QFgame4cost = Q1groupDcost;
        QFgame4pop = Q1groupDpop;
        QFgame45 = Q1groupD5;
        QFgame4C5 = Q1groupDC5;
        QFgame4V5 = Q1groupDV5;
        QFgame4D5 = Q1groupDD5;
        
        FQFgame4 = FQ1groupD;
        
    }

    //game 5
    if (Q1groupE > Q2groupF) {
        cout << FQ1groupE <<" won "<< FQ2groupF << " in round 1" << endl;
        QFgame5 = Q1groupE;
        QFgame5attack = Q1groupEattack;
        QFgame5midfield = Q1groupEmidfield;
        QFgame5deffence = Q1groupEdeffence;
        QFgame5f = Q1groupEf;
        QFgame5cost = Q1groupEcost;
        QFgame5pop = Q1groupEpop;
        QFgame55 = Q1groupE5;
        QFgame5C5 = Q1groupEC5;
        QFgame5V5 = Q1groupEV5;
        QFgame5D5 = Q1groupED5;
        
        FQFgame5 = FQ1groupE;
        
    }

    if (Q1groupE < Q2groupF) {
        cout << FQ2groupF <<" won "<< FQ1groupE << " in round 1" << endl;
        QFgame5 = Q2groupF;
        QFgame5attack = Q2groupFattack;
        QFgame5midfield = Q2groupFmidfield;
        QFgame5deffence = Q2groupFdeffence;
        QFgame5f = Q2groupFf;
        QFgame5cost = Q2groupFcost;
        QFgame5pop = Q2groupFpop;
        QFgame55 = Q2groupF5;
        QFgame5C5 = Q2groupFC5;
        QFgame5V5 = Q2groupFV5;
        QFgame5D5 = Q2groupFD5;
        
        FQFgame5 = FQ2groupF;
        
    }

    //game 6
    if (Q2groupE > Q1groupF) {
        cout << FQ2groupE <<" won "<< FQ1groupF << " in round 1" << endl;
        QFgame6 = Q2groupE;
        QFgame6attack = Q2groupEattack;
        QFgame6midfield = Q2groupEmidfield;
        QFgame6deffence = Q2groupEdeffence;
        QFgame6f = Q2groupEf;
        QFgame6cost = Q2groupEcost;
        QFgame6pop = Q2groupEpop;
        QFgame65 = Q2groupE5;
        QFgame6C5 = Q2groupEC5;
        QFgame6V5 = Q2groupEV5;
        QFgame6D5 = Q2groupED5;
        
        FQFgame6 = FQ2groupE;
        
    }

    if (Q2groupE < Q1groupF) {
        cout << FQ1groupF <<" won "<< FQ2groupE << " in round 1" << endl;
        QFgame6 = Q1groupF;
        QFgame6attack = Q1groupFattack;
        QFgame6midfield = Q1groupFmidfield;
        QFgame6deffence = Q1groupFdeffence;
        QFgame6f = Q1groupFf;
        QFgame6cost = Q1groupFcost;
        QFgame6pop = Q1groupFpop;
        QFgame65 = Q1groupF5;
        QFgame6C5 = Q1groupFC5;
        QFgame6V5 = Q1groupFV5;
        QFgame6D5 = Q1groupFD5;
        
        FQFgame6 = FQ1groupF;
        
    }

    //game 7
    if (Q1groupG > Q2groupH) {
        cout << FQ1groupG <<" won "<< FQ2groupH << " in round 1" << endl;
        QFgame7 = Q1groupG;
        QFgame7attack = Q1groupGattack;
        QFgame7midfield = Q1groupGmidfield;
        QFgame7deffence = Q1groupGdeffence;
        QFgame7f = Q1groupGf;
        QFgame7cost = Q1groupGcost;
        QFgame7pop = Q1groupGpop;
        QFgame75 = Q1groupG5;
        QFgame7C5 = Q1groupGC5;
        QFgame7V5 = Q1groupGV5;
        QFgame7D5 = Q1groupGD5;
        
        FQFgame7 = FQ1groupG;
        
    }

    if (Q1groupG < Q2groupH) {
        cout << FQ2groupH <<" won "<< FQ1groupG << " in round 1" << endl;
        QFgame7 = Q2groupH;
        QFgame7attack = Q2groupHattack;
        QFgame7midfield = Q2groupHmidfield;
        QFgame7deffence = Q2groupHdeffence;
        QFgame7f = Q2groupHf;
        QFgame7cost = Q2groupHcost;
        QFgame7pop = Q2groupHpop;
        QFgame75 = Q2groupH5;
        QFgame7C5 = Q2groupHC5;
        QFgame7V5 = Q2groupHV5;
        QFgame7D5 = Q2groupHD5;
        
        FQFgame7 = FQ2groupH;
        
    }

    //game 8
    if (Q2groupG > Q1groupH) {
        cout << FQ2groupG <<" won "<< FQ1groupH << " in round 1" << endl;
        QFgame8 = Q2groupG;
        QFgame8attack = Q2groupGattack;
        QFgame8midfield = Q2groupGmidfield;
        QFgame8deffence = Q2groupGdeffence;
        QFgame8f = Q2groupGf;
        QFgame8cost = Q2groupGcost;
        QFgame8pop = Q2groupGpop;
        QFgame85 = Q2groupG5;
        QFgame8C5 = Q2groupGC5;
        QFgame8V5 = Q2groupGV5;
        QFgame8D5 = Q2groupGD5;
        
        FQFgame8 = FQ2groupG;
        
    }

    if (Q2groupG < Q1groupH) {
        cout << FQ1groupH <<" won "<< FQ2groupG << " in round 1" << endl;
        QFgame8 = Q1groupH;
        QFgame8attack = Q1groupHattack;
        QFgame8midfield = Q1groupHmidfield;
        QFgame8deffence = Q1groupHdeffence;
        QFgame8f = Q1groupHf;
        QFgame8cost = Q1groupHcost;
        QFgame8pop = Q1groupHpop;
        QFgame85 = Q1groupH5;
        QFgame8C5 = Q1groupHC5;
        QFgame8V5 = Q1groupHV5;
        QFgame8D5 = Q1groupHD5;
        
        FQFgame8 = FQ1groupH;
        
    }

    //After the compiler decides who won the rounds, the teams will then undergo another simulation in which we'll get to know who won the quater finals

    //Comparison of quarter-finals teams' attack

    //Game one's comparison

    //Attack
    if (QFgame1attack > QFgame3attack) {
        QFgame1 += 8;
    }

    else if (QFgame1attack < QFgame3attack) {
        QFgame3 += 8;
    }
    //midfield
    if (QFgame1midfield > QFgame3midfield) {
        QFgame1 += 8;
    }

    else if (QFgame1midfield < QFgame3midfield) {
        QFgame3 += 8;
    }

    //deffence
    if (QFgame1deffence > QFgame3deffence) {
        QFgame1 += 8;
    }

    else if (QFgame1deffence < QFgame3deffence) {
        QFgame3 += 8;
    }

    //factor of unexpectancy
    if (QFgame1f > QFgame3f) {
        QFgame1 += 1;
    }

    else if (QFgame1f < QFgame3f) {
        QFgame3 += 1;
    }

    //cost of teams
    if (QFgame1cost > QFgame3cost) {
        QFgame1 += 5;
    }

    else if (QFgame1cost < QFgame3cost) {
        QFgame3 += 5;
    }

    //popuplation
    if (QFgame1pop > QFgame3pop) {
        QFgame1 += 5;
    }

    else if (QFgame1pop < QFgame3pop) {
        QFgame3 += 5;
    }

    //# of goals score in last 5 games
    if (QFgame15 > QFgame35) {
        QFgame1 += 1;
    }

    else if (QFgame15 < QFgame35) {
        QFgame3 += 1;
    }

    //# of goals conceded in last 5 games
    if (QFgame1C5 > QFgame3C5) {
        QFgame1 -= 1;
    }

    else if (QFgame1C5 < QFgame3C5) {
        QFgame3 -= 1;
    }

    //# of victories in last 5 games
    if (QFgame1V5 > QFgame3V5) {
        QFgame1 += 1;
    }

    else if (QFgame1V5 < QFgame3V5) {
        QFgame3 += 1;
    }

    //# of defeats in last 5 games
    if (QFgame1D5 > QFgame3D5) {
        QFgame1 -= 1;
    }

    else if (QFgame1D5 < QFgame3D5) {
        QFgame3 -= 1;
    }

     
    //Game two's comparison
    //Attack
    if (QFgame5attack > QFgame7attack) {
        QFgame5 += 8;
    }

    else if (QFgame5attack < QFgame7attack) {
        QFgame7 += 8;
    }
    //midfield
    if (QFgame5midfield > QFgame7attack) {
        QFgame5 += 8;
    }

    else if (QFgame5midfield < QFgame7attack) {
        QFgame7 += 8;
    }

    //deffence
    if (QFgame5deffence > QFgame7deffence) {
        QFgame5 += 8;
    }

    else if (QFgame5deffence < QFgame7deffence) {
        QFgame7 += 8;
    }

    //factor of unexpectancy
    if (QFgame5f > QFgame7f) {
        QFgame5 += 1;
    }

    else if (QFgame5f < QFgame7f) {
        QFgame7 += 1;
    }

    //cost of teams
    if (QFgame5cost > QFgame7cost) {
        QFgame5 += 5;
    }

    else if (QFgame5cost < QFgame7cost) {
        QFgame7 += 5;
    }

    //popuplation
    if (QFgame5pop > QFgame7pop) {
        QFgame5 += 5;
    }

    else if (QFgame5pop < QFgame7pop) {
        QFgame7 += 5;
    }

    //# of goals score in last 5 games
    if (QFgame55 > QFgame75) {
        QFgame5 += 1;
    }

    else if (QFgame55 < QFgame75) {
        QFgame7 += 1;
    }

    //# of goals conceded in last 5 games
    if (QFgame5C5 > QFgame7C5) {
        QFgame5 -= 1;
    }

    else if (QFgame5C5 < QFgame7C5) {
        QFgame7 -= 1;
    }

    //# of victories in last 5 games
    if (QFgame5V5 > QFgame7V5) {
        QFgame5 += 1;
    }

    else if (QFgame5V5 < QFgame7V5) {
        QFgame7 += 1;
    }

    //# of defeats in last 5 games
    if (QFgame5D5 > QFgame7D5) {
        QFgame5 -= 1;
    }

    else if (QFgame5D5 < QFgame7D5) {
        QFgame7 -= 1;
    }

    
    //Game three's comparison
    //Attack
    if (QFgame2attack > QFgame4attack) {
        QFgame2 += 8;
    }

    else if (QFgame2attack < QFgame4attack) {
        QFgame4 += 8;
    }

    //midfield
    if (QFgame2midfield > QFgame4midfield) {
        QFgame2 += 8;
    }

    else if (QFgame2midfield < QFgame4midfield) {
        QFgame4 += 8;
    }

    //deffence
    if (QFgame2deffence > QFgame4deffence) {
        QFgame2 += 8;
    }

    else if (QFgame2deffence < QFgame4deffence) {
        QFgame4 += 8;
    }

    //factor of unexpectancy
    if (QFgame2f > QFgame4f) {
        QFgame2 += 1;
    }

    else if (QFgame2f < QFgame4f) {
        QFgame4 += 1;
    }

    //cost of teams
    if (QFgame2cost > QFgame4cost) {
        QFgame2 += 5;
    }

    else if (QFgame2cost < QFgame4cost) {
        QFgame4 += 5;
    }

    //popuplation
    if (QFgame2pop > QFgame4pop) {
        QFgame2 += 5;
    }

    else if (QFgame2pop < QFgame4pop) {
        QFgame4 += 5;
    }

    //# of goals score in last 5 games
    if (QFgame25 > QFgame45) {
        QFgame2 += 1;
    }

    else if (QFgame25 < QFgame45) {
        QFgame4 += 1;
    }


    //# of goals conceded in last 5 games
    if (QFgame2C5 > QFgame4C5) {
        QFgame2 -= 1;
    }

    else if (QFgame2C5 < QFgame4C5) {
        QFgame4 -= 1;
    }

    //# of victories in last 5 games
    if (QFgame2V5 > QFgame4V5) {
        QFgame2 += 1;
    }

    else if (QFgame2V5 < QFgame4V5) {
        QFgame4 += 1;
    }

    //# of defeats in last 5 games
    if (QFgame2D5 > QFgame4D5) {
        QFgame2 -= 1;
    }

    else if (QFgame2D5 < QFgame4D5) {
        QFgame4 -= 1;
    }

    
    //Game four's comparison
    //Attack
    if (QFgame6attack > QFgame8attack) {
        QFgame6 += 8;
    }

    else if (QFgame6attack < QFgame8attack) {
        QFgame8 += 8;
    }

    //midfield
    if (QFgame6midfield > QFgame8midfield) {
        QFgame6 += 8;
    }

    else if (QFgame6midfield < QFgame8midfield) {
        QFgame8 += 8;
    }

    //deffence
    if (QFgame6deffence > QFgame8deffence) {
        QFgame6 += 8;
    }

    else if (QFgame6deffence < QFgame8deffence) {
        QFgame8 += 8;
    }

    //factor of unexpectancy
    if (QFgame6f > QFgame8f) {
        QFgame6 += 1;
    }

    else if (QFgame6f < QFgame8f) {
        QFgame8 += 1;
    }

    //cost of teams
    if (QFgame6cost > QFgame8cost) {
        QFgame6 += 5;
    }

    else if (QFgame6cost < QFgame8cost) {
        QFgame8 += 5;
    }

    //popuplation
    if (QFgame6pop > QFgame8pop) {
        QFgame6 += 5;
    }

    else if (QFgame6pop < QFgame8pop) {
        QFgame8 += 5;
    }

    //# of goals score in last 5 games
    if (QFgame65 > QFgame85) {
        QFgame6 += 1;
    }

    else if (QFgame65 < QFgame85) {
        QFgame8 += 1;
    }

    //# of goals conceded in last 5 games
    if (QFgame6C5 > QFgame8C5) {
        QFgame6 -= 1;
    }

    else if (QFgame6C5 < QFgame8C5) {
        QFgame8 -= 1;
    }

    //# of victories in last 5 games
    if (QFgame6V5 > QFgame8V5) {
        QFgame6 += 1;
    }

    else if (QFgame6V5 < QFgame8V5) {
        QFgame8 += 1;
    }

    //# of defeats in last 5 games
    if (QFgame6D5 > QFgame8D5) {
        QFgame6 -= 1;
    }

    else if (QFgame6D5 < QFgame8D5) {
        QFgame8 -= 1;
    }

   
    cout << endl;
    
    //The following code will ouput the results of the quater finals. There are 4 games.

    //Quarter-finals match results
    //game 1
    if (QFgame1 > QFgame3) {
        cout << FQFgame1 <<" won "<< FQFgame3 << " quarter-finals game 1" << endl;
        SFgame1 = QFgame1;
        SFgame1attack = QFgame1attack;
        SFgame1midfield = QFgame1midfield;
        SFgame1deffence = QFgame1deffence;
        SFgame1f = QFgame1f;
        SFgame1cost = QFgame1cost;
        SFgame1pop = QFgame1pop;
        SFgame15 = QFgame15;
        SFgame1C5 = QFgame1C5;
        SFgame1V5 = QFgame1V5;
        SFgame1D5 = QFgame1D5;
        
        FSFgame1 = FQFgame1;
        
    }

    if (QFgame1 < QFgame3) {
        cout << FQFgame3 <<" won "<< FQFgame1 << " quarter-finals game 1" << endl;
        SFgame1 = QFgame3;
        SFgame1attack = QFgame3attack;
        SFgame1midfield = QFgame3midfield;
        SFgame1deffence = QFgame3deffence;
        SFgame1f = QFgame3f;
        SFgame1cost = QFgame3cost;
        SFgame1pop = QFgame3pop;
        SFgame15 = QFgame35;
        SFgame1C5 = QFgame3C5;
        SFgame1V5 = QFgame3V5;
        SFgame1D5 = QFgame3D5;
        
        FSFgame1 = FQFgame3;
        
    }

    //game 2
    if (QFgame5 > QFgame7) {
        cout << FQFgame5 <<" won "<< FQFgame7 << " quarter-finals game 2" << endl;
        SFgame2 = QFgame5;
        SFgame2attack = QFgame5attack;
        SFgame2midfield = QFgame5midfield;
        SFgame2deffence = QFgame5deffence;
        SFgame2f = QFgame5f;
        SFgame2cost = QFgame5cost;
        SFgame2pop = QFgame5pop;
        SFgame25 = QFgame55;
        SFgame2C5 = QFgame5C5;
        SFgame2V5 = QFgame5V5;
        SFgame2D5 = QFgame5D5;
        
        FSFgame2 = FQFgame5;
        
    }

    if (QFgame5 < QFgame7) {
        cout << FQFgame7 <<" won "<< FQFgame5 << " quarter-finals game 2" << endl;
        SFgame2 = QFgame7;
        SFgame2attack = QFgame7attack;
        SFgame2midfield = QFgame7midfield;
        SFgame2deffence = QFgame7deffence;
        SFgame2f = QFgame7f;
        SFgame2cost = QFgame7cost;
        SFgame2pop = QFgame7pop;
        SFgame25 = QFgame75;
        SFgame2C5 = QFgame7C5;
        SFgame2V5 = QFgame7V5;
        SFgame2D5 = QFgame7D5;
        
        FSFgame2 = FQFgame7;
        
    }

    //game 3
    if (QFgame2 > QFgame4) {
        cout << FQFgame2 <<" won "<< FQFgame4 << " quarter-finals game 3" << endl;
        SFgame3 = QFgame2;
        SFgame3attack = QFgame2attack;
        SFgame3midfield = QFgame2midfield;
        SFgame3deffence = QFgame2deffence;
        SFgame3f = QFgame2f;
        SFgame3cost = QFgame2cost;
        SFgame3pop = QFgame2pop;
        SFgame35 = QFgame25;
        SFgame3C5 = QFgame2C5;
        SFgame3V5 = QFgame2V5;
        SFgame3D5 = QFgame2D5;
        
        FSFgame3 = FQFgame2;
        
    }

    if (QFgame2 < QFgame4) {
        cout << FQFgame4 <<" won "<< FQFgame2 << " quarter-finals game 3" << endl;
        SFgame3 = QFgame4;
        SFgame3attack = QFgame4attack;
        SFgame3midfield = QFgame4midfield;
        SFgame3deffence = QFgame4deffence;
        SFgame3f = QFgame4f;
        SFgame3cost = QFgame4cost;
        SFgame3pop = QFgame4pop;
        SFgame35 = QFgame45;
        SFgame3C5 = QFgame4C5;
        SFgame3V5 = QFgame4V5;
        SFgame3D5 = QFgame4D5;
        
        FSFgame3 = FQFgame4;
        
    }

    //game 4
    if (QFgame6 > QFgame8) {
        cout << FQFgame6 <<" won "<< FQFgame8 << " quarter-finals game 4" << endl;
        SFgame4 = QFgame6;
        SFgame4attack = QFgame6attack;
        SFgame4midfield = QFgame6midfield;
        SFgame4deffence = QFgame6deffence;
        SFgame4f = QFgame6f;
        SFgame4cost = QFgame6cost;
        SFgame4pop = QFgame6pop;
        SFgame45 = QFgame65;
        SFgame4C5 = QFgame6C5;
        SFgame4V5 = QFgame6V5;
        SFgame4D5 = QFgame6D5;
        
        FSFgame4 = FQFgame6;
        
    }

    if (QFgame6 < QFgame8) {
        cout << FQFgame8 <<" won "<< FQFgame6 << " quarter-finals game 4" << endl;
        SFgame4 = QFgame8;
        SFgame4attack = QFgame8attack;
        SFgame4midfield = QFgame8midfield;
        SFgame4deffence = QFgame8deffence;
        SFgame4f = QFgame8f;
        SFgame4cost = QFgame8cost;
        SFgame4pop = QFgame8pop;
        SFgame45 = QFgame85;
        SFgame4C5 = QFgame8C5;
        SFgame4V5 = QFgame8V5;
        SFgame4D5 = QFgame8D5;
        
        FSFgame4 = FQFgame8;
        
    }

    //After the quarter finals comes the semi finals. In the previous part of the code, the compiler outputs the winners of quarter finals and now in this part, the compiler will compete against those two teams and decide who is going to the finals 

    //Comparison of semi-finals teams' attack

    //Game one's comparison

    //Attack
    if (SFgame1attack > SFgame2attack) {
        SFgame1 += 10;
    }

    else if (SFgame1attack < SFgame2attack) {
        SFgame2 += 10;
    }

    //midfield
    if (SFgame1midfield > SFgame2midfield) {
        SFgame1 += 10;
    }

    else if (SFgame1midfield < SFgame2midfield) {
        SFgame2 += 10;
    }

    //deffence
    if (SFgame1deffence > SFgame2deffence) {
        SFgame1 += 10;
    }

    else if (SFgame1deffence < SFgame2deffence) {
        SFgame2 += 10;
    }

    //factor of unexpectancy
    if (SFgame1f > SFgame2f) {
        SFgame1 += 1;
    }

    else if (SFgame1f < SFgame2f) {
        SFgame2 += 1;
    }

    //cost of teams
    if (SFgame1cost > SFgame2cost) {
        SFgame1 += 6;
    }

    else if (SFgame1cost < SFgame2cost) {
        SFgame2 += 6;
    }

    //population
    if (SFgame1pop > SFgame2pop) {
        SFgame1 += 6;
    }

    else if (SFgame1pop < SFgame2pop) {
        SFgame2 += 6;
    }

    //# of goals score in last 5 games
    if (SFgame15 > SFgame25) {
        SFgame1 += 1;
    }

    else if (SFgame15 < SFgame25) {
        SFgame2 += 1;
    }

    //# of goals conceded in last 5 games
    if (SFgame1C5 > SFgame2C5) {
        SFgame1 -= 1;
    }

    else if (SFgame1C5 < SFgame2C5) {
        SFgame2 -= 1;
    }

    //# of victories in last 5 games
    if (SFgame1V5 > SFgame2V5) {
        SFgame1 += 1;
    }

    else if (SFgame1V5 < SFgame2V5) {
        SFgame2 += 1;
    }

    //# of defeats in last 5 games
    if (SFgame1D5 > SFgame2D5) {
        SFgame1 -= 1;
    }

    else if (SFgame1D5 < SFgame2D5) {
        SFgame2 -= 1;
    }

    
    //Game two's comparison
    //Attack
    if (SFgame3attack > SFgame4attack) {
        SFgame3 += 10;
    }

    else if (SFgame3attack < SFgame4attack) {
        SFgame4 += 10;
    }

    //midfield
    if (SFgame3midfield > SFgame4midfield) {
        SFgame3 += 10;
    }

    else if (SFgame3midfield < SFgame4midfield) {
        SFgame4 += 10;
    }

    //deffence
    if (SFgame3deffence > SFgame4deffence) {
        SFgame3 += 10;
    }

    else if (SFgame3deffence < SFgame4deffence) {
        SFgame4 += 10;
    }

    //factor of unexpectancy
    if (SFgame3f > SFgame4f) {
        SFgame3 += 1;
    }

    else if (SFgame3f < SFgame4f) {
        SFgame4 += 1;
    }

    //cost of teams
    if (SFgame3cost > SFgame4cost) {
        SFgame3 += 6;
    }

    else if (SFgame3cost < SFgame4cost) {
        SFgame4 += 6;
    }

    //popuplation
    if (SFgame3pop > SFgame4pop) {
        SFgame3 += 6;
    }

    else if (SFgame3pop < SFgame4pop) {
        SFgame4 += 6;
    }

    //# of goals score in last 5 games
    if (SFgame35 > SFgame45) {
        SFgame3 += 1;
    }

    else if (SFgame35 < SFgame45) {
        SFgame4 += 1;
    }

    //# of goals conceded in last 5 games
    if (SFgame3C5 > SFgame4C5) {
        SFgame3 -= 1;
    }

    else if (SFgame3C5 < SFgame4C5) {
        SFgame4 -= 1;
    }

    //# of victories in last 5 games
    if (SFgame3V5 > SFgame4V5) {
        SFgame3 += 1;
    }

    else if (SFgame3V5 < SFgame4V5) {
        SFgame4 += 1;
    }

    //# of defeats in last 5 games
    if (SFgame3D5 > SFgame4D5) {
        SFgame3 -= 1;
    }

    else if (SFgame3D5 < SFgame4D5) {
        SFgame4 -= 1;
    }

    cout << endl;

    //Now the compiler is going to output the results of semi finals based upon the factors.
    
    //Semi-finals match results
    //game 1
    if (SFgame1 > SFgame2) {
        cout << FSFgame1 <<" won "<< FSFgame2 << " in semi-finals game 1" << endl;
        R1game1F = SFgame1;
        R1game1Fattack = SFgame1attack;
        R1game1Fmidfield = SFgame1midfield;
        R1game1Fdeffence = SFgame1deffence;
        R1game1Ff = SFgame1f;
        R1game1Fcost = SFgame1cost;
        R1game1Fpop = SFgame1pop;
        R1game1F5 = SFgame15;
        R1game1FC5 = SFgame1C5;
        R1game1FV5 = SFgame1V5;
        R1game1FD5 = SFgame1D5;

        R1game1T = SFgame2;
        R1game1Tattack = SFgame2attack;
        R1game1Tmidfield = SFgame2midfield;
        R1game1Tdeffence = SFgame2deffence;
        R1game1Tf = SFgame2f;
        R1game1Tcost = SFgame2cost;
        R1game1Tpop = SFgame2pop;
        R1game1T5 = SFgame25;
        R1game1TC5 = SFgame2C5;
        R1game1TV5 = SFgame2V5;
        R1game1TD5 = SFgame2D5;
        
        FR1game1F = FSFgame1;
        FR1game1T = FSFgame2;
    }

    if (SFgame1 < SFgame2) {
        cout << FSFgame2 <<" won "<< FSFgame1 << " in semi-finals game 1" << endl;
        R1game1T = SFgame1;
        R1game1Tattack = SFgame1attack;
        R1game1Tmidfield = SFgame1midfield;
        R1game1Tdeffence = SFgame1deffence;
        R1game1Tf = SFgame1f;
        R1game1Tcost = SFgame1cost;
        R1game1Tpop = SFgame1pop;
        R1game1T5 = SFgame15;
        R1game1TC5 = SFgame1C5;
        R1game1TV5 = SFgame1V5;
        R1game1TD5 = SFgame1D5;
       
        R1game1F = SFgame2;
        R1game1Fattack = SFgame2attack;
        R1game1Fmidfield = SFgame2midfield;
        R1game1Fdeffence = SFgame2deffence;
        R1game1Ff = SFgame2f;
        R1game1Fcost = SFgame2cost;
        R1game1Fpop = SFgame2pop;
        R1game1F5 = SFgame25;
        R1game1FC5 = SFgame2C5;
        R1game1FV5 = SFgame2V5;
        R1game1FD5 = SFgame2D5;

        
        FR1game1T = FSFgame1;
        FR1game1F = FSFgame2;
    }


    //game 2
    if (SFgame3 > SFgame4) {
        cout << FSFgame3 <<" won "<< FSFgame4 << " in semi-finals game 2" << endl;
        R1game2F = SFgame3;
        R1game2Fattack = SFgame3attack;
        R1game2Fmidfield = SFgame3midfield;
        R1game2Fdeffence = SFgame3deffence;
        R1game2Ff = SFgame3f;
        R1game2Fcost = SFgame3cost;
        R1game2Fpop = SFgame3pop;
        R1game2F5 = SFgame35;
        R1game2FC5 = SFgame3C5;
        R1game2FV5 = SFgame3V5;
        R1game2FD5 = SFgame3D5;


       
        R1game2T = SFgame4;
        R1game2Tattack = SFgame4attack;
        R1game2Tmidfield = SFgame4midfield;
        R1game2Tdeffence = SFgame4deffence;
        R1game2Tf = SFgame4f;
        R1game2Tcost = SFgame4cost;
        R1game2Tpop = SFgame4pop;
        R1game2T5 = SFgame45;
        R1game2TC5 = SFgame4C5;
        R1game2TV5 = SFgame4V5;
        R1game2TD5 = SFgame4D5;

        
        FR1game2F = FSFgame3;
        FR1game2T = FSFgame4;
    }

    if (SFgame3 < SFgame4) {
        cout << FSFgame4 <<" won "<< FSFgame3 << " in semi-finals game 2" << endl;
        R1game2T = SFgame3;
        R1game2Tattack = SFgame3attack;
        R1game2Tmidfield = SFgame3midfield;
        R1game2Tdeffence = SFgame3deffence;
        R1game2Tf = SFgame3f;
        R1game2Tcost = SFgame3cost;
        R1game2Tpop = SFgame3pop;
        R1game2T5 = SFgame35;
        R1game2TC5 = SFgame3C5;
        R1game2TV5 = SFgame3V5;
        R1game2TD5 = SFgame3D5;


       
        R1game2F = SFgame4;
        R1game2Fattack = SFgame4attack;
        R1game2Fmidfield = SFgame4midfield;
        R1game2Fdeffence = SFgame4deffence;
        R1game2Ff = SFgame4f;
        R1game2Fcost = SFgame4cost;
        R1game2Fpop = SFgame4pop;
        R1game2F5 = SFgame45;
        R1game2FC5 = SFgame4C5;
        R1game2FV5 = SFgame4V5;
        R1game2FD5 = SFgame4D5;

        
        FR1game2T = FSFgame3;
        FR1game2F = FSFgame4;
    }

    //Now, the compiler has given us the output on which team is the winner of semi finals and now the compiler will decide which team is going to participate and win the finals

    //Finals (comparing every factors)
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

    //factor of unexpectancy
    if (R1game1Ff > R1game2Ff) {
        R1game1F += 1;
    }

    else if (R1game1Ff < R1game2Ff) {
        R1game2F += 1;
    }

    //cost of teams
    if (R1game1Fcost > R1game2Fcost) {
        R1game1F += 1;
    }

    else if (R1game1Fcost < R1game2Fcost) {
        R1game2F += 1;
    }

    //popuplation
    if (R1game1Fpop > R1game2Fpop) {
        R1game1F += 1;
    }

    else if (R1game1Fpop < R1game2Fpop) {
        R1game2F += 1;
    }

    //# of goals score in last 5 games
    if (R1game1F5 > R1game2F5) {
        R1game1F += 1;
    }

    else if (R1game1F5 < R1game2F5) {
        R1game2F += 1;
    }

    //# of goals conceded in last 5 games
    if (R1game1FC5 > R1game2FC5) {
        R1game1F -= 1;
    }

    else if (R1game1FC5 < R1game2FC5) {
        R1game2F -= 1;
    }

    //# of victories in last 5 games
    if (R1game1FV5 > R1game2FV5) {
        R1game1F += 1;
    }

    else if (R1game1FV5 < R1game2FV5) {
        R1game2F += 1;
    }

    //# of defeats in last 5 games
    if (R1game1FD5 > R1game2FD5) {
        R1game1F -= 1;
    }

    else if (R1game1FD5 < R1game2FD5) {
        R1game2F -= 1;
    }

    
    //Third Place
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

    //factor of unexpectancy
    if (R1game1Tf > R1game2Tf) {
        R1game1T += 1;
    }

    else if (R1game1Tf < R1game2Tf) {
        R1game2T += 1;
    }

    //cost of teams
    if (R1game1Tcost > R1game2Tcost) {
        R1game1T += 1;
    }

    else if (R1game1Tcost < R1game2Tcost) {
        R1game2T += 1;
    }

    //popuplation
    if (R1game1Tpop > R1game2Tpop) {
        R1game1T += 1;
    }

    else if (R1game1Tpop < R1game2Tpop) {
        R1game2T += 1;
    }

    //# of goals score in last 5 games
    if (R1game1T5 > R1game2T5) {
        R1game1T += 1;
    }

    else if (R1game1T5 < R1game2T5) {
        R1game2T += 1;
    }

    //# of goals conceded in last 5 games
    if (R1game1TC5 > R1game2TC5) {
        R1game1T -= 1;
    }

    else if (R1game1TC5 < R1game2TC5) {
        R1game2T -= 1;
    }

    //# of victories in last 5 games
    if (R1game1TV5 > R1game2TV5) {
        R1game1T += 1;
    }

    else if (R1game1TV5 < R1game2TV5) {
        R1game2T += 1;
    }

    //# of defeats in last 5 games
    if (R1game1TD5 > R1game2TD5) {
        R1game1T -= 1;
    }

    else if (R1game1TD5 < R1game2TD5) {
        R1game2T -= 1;
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
    
    
//The compiler not only tells who the winner of the tournament is but also tells us the team who is standing at 2nd and 3rd place.

//In the following code, we have also included a factor called 'factor of unexpectancy'. As this tournament is based on real team statistics
// and in real life we never know which team will win. Even the strongest teams can lose and that's why we included the 'factor of unexpectancy'. 

//The usage of random number generator is helpful in this factor as this is the only thing which the compiler decides randomly. Everything else the
// compiler decides is due to the actual statistic we input in the code.



    


















}
