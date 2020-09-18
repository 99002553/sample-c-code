# sample-c-code

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/4fe2125c1a434784ae4dd5776d4ef852)](https://app.codacy.com/manual/stepin104698/sample-c-code?utm_source=github.com&utm_medium=referral&utm_content=stepin104698/sample-c-code&utm_campaign=Badge_Grade_Dashboard)

#my first repository on github
#include<stdio.h>
#include<conio.h>
intvalid(intnum);
int flag;
FILE *fp;
char ch[150];
void main()
{
int s=0,c=0,a=0;
intans;
clrscr();
printf("BALLARI INSTITUTE OF TECHNOLOGY AND MANAGEMENT\n");
printf("welcome to career guidence management\n");

printf("here is the questionnaire\n");
printf("study of universe is known as?\n");
printf("1.socology\t2.cosmology\n3.universology\t4.petology\t\n");

scanf("%d",&ans);
flag=valid(ans);
if(flag==1)
{
if(ans==2)
s++;
}
printf("which planet is dwarf planet \n");
printf("1.mercury\t2.pluto\n3.mars\t4.uranus\t\n");
scanf("%d",&ans);
flag=valid(ans);
if(flag==1)
{
if(ans==2)
s++;
}
printf("floods can be prevented by\n");
printf("1.afforestation\t2.removing top soil\n3.deforestation\t4.none of the above\n");
scanf("%d",&ans);
flag=valid(ans);
if(flag==1)
{
if(ans==2)
s++;
}
printf("which of the following is a green house gas\n");
printf("1.nitrogen dioxide\t2.sulphur dioxide\n3.carbon dioxide\t4.carbon monoxide\n");
scanf("%d",&ans);
flag=valid(ans);
if(flag==1)
{
if(ans==3)
s++;
}
printf("narmadabachaoandlan was to clean narmada\n");
printf("1.clean narmada\t2.expand narmada\n3.sava narmada\t4.none of the above\n");
scanf("%d",&ans);
flag=valid(ans);
if(flag==1)
{
if(ans==3)
s++;
}
printf("every quadractic polynomial can have almost \n");
printf("1.three zero's\t2.one zero\n3.two zero's\t4.none of the above\t\n");
scanf("%d",&ans);
flag=valid(ans);
if(flag==1)
{
if(ans==3)
c++;
}
printf("gramina bank is a succes story of ?\n");
printf("1.india\tbangladesh\n3.nepal\t4.china\t\n");
scanf("%d",&ans);
flag=valid(ans);
if(flag==1)
{
if(ans==2)
c++;
}
printf("journalist who _________ detained in a city for more than  year \n");
printf("1.is be\t2.can be\n3.might been\t4has been\n");
scanf("%d",&ans);
flag=valid(ans);
if(flag==1)
{
if(ans==4)
c++;
}
printf(" banks donot give loans for?\n");
printf("1.to small framers\t2.marginal farmers\n3.to industries\t4.none of the above\n");
scanf("%d",&ans);
flag=valid(ans);
if(flag==1)
{
if(ans==4)
c++;
}
printf("which of the can be considered as a modern forms of money\n");
printf("1.currencies\t2.drafts\n3.cheques\t4.all of the above\n");
scanf("%d",&ans);
flag=valid(ans);
if(flag==1)
{
if(ans==4)
c++;
}
printf("overlapping of two primary colors form\n");
printf("1.teritary color\t2.mixed color\n3.secondary color\t4.both\t\n");
scanf("%d",&ans);
flag=valid(ans);
if(flag==1)
{
if(ans==4)
a++;
}
printf("tyebmehta is famous for ?\n");
printf("1.writer\t2.painter\t3.singer\t4.cartoonist\t\n");
scanf("%d",&ans);
flag=valid(ans);
if(flag==1)
{
if(ans==2)
a++;
}
printf("when red and blue are combined together they form\n");
printf("1.blue\t2.magentha\n3.orange\t4.purple\n");
scanf("%d",&ans);
flag=valid(ans);
if(flag==1)
{
if(ans==2)
a++;
}
printf("which of the following dance is not from punjab\n");
printf("1.gidda\t2.tamasha\n3.bhangra\t4.bhand\n");
scanf("%d" ,&ans);
flag=valid(ans);
if(flag==1)
{
if(ans==2)
a++;
}
printf("who invented sitar\n");
printf("1.amir khusro\t2.bahadur shazafar\n3.ali akbar khan\t4.none of the above\t");
scanf("%d",&ans);
flag=valid(ans);
if(flag==1)
{
if(ans==1)
a++;
}
if((s>c)&&(s>a))
{
fp=fopen("a.txt","r");
if(fp==NULL)
{
printf("cannot open file\n");
exit(0);
}
while(fgets(ch,10,fp)!=NULL)
{
//fscanf(fp,"%s",ch);
printf("%s",ch);
}
fclose(fp);
}
else if(c>a)
{
fp=fopen("b.txt","r");
if(fp==NULL)
{
printf("cannot open file\n");
exit(0);
}
while(fgets(ch,10,fp)!=NULL)
{
//fscanf(fp,"%s",ch);
printf("%s",ch);
}
fclose(fp);
}
else
{
fp=fopen("c.txt","r");
if(fp==NULL)
{
printf("cannot open file\n");
exit(0);
}
while(fgets(ch,10,fp)!=NULL)
{
//fscanf(fp,"%s",ch);
printf("%s",ch);
}
fclose(fp);
}
getch();
}

intvalid(intnum)
{
if((num==1)||(num==2)||(num==3)||(num==4))
{
flag=1;
return(flag);
}
else
{
printf ("invalid option\n");
printf ("enter your option again\n");
scanf("%d",&num);
valid(num);
}
return 0;
}

