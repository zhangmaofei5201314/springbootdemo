PK  ��VO               meta.xml'��<?xml version="1.0" encoding="UTF-8" standalone="no"?><meta xmlns="urn:xmind:xmap:xmlns:meta:2.0" version="2.0"><Thumbnail><Origin><X>541</X><Y>166</Y></Origin><BackgroundColor>#F3F4F9</BackgroundColor></Thumbnail><Creator><Name>XMind</Name><Version>3.5.1.201411201906</Version></Creator></meta>PKiwQ,  '  PK  ��VO               content.xmlC��<?xml version="1.0" encoding="UTF-8" standalone="no"?><xmap-content xmlns="urn:xmind:xmap:xmlns:content:2.0" xmlns:fo="http://www.w3.org/1999/XSL/Format" xmlns:svg="http://www.w3.org/2000/svg" xmlns:xhtml="http://www.w3.org/1999/xhtml" xmlns:xlink="http://www.w3.org/1999/xlink" timestamp="1571736575064" version="2.0"><sheet id="4c8cdrtv5uli10r8nr70grk327" style-id="3b7n6l540kiaagavceovs7toh1" theme="xminddefaultthemeid2014" timestamp="1571736575064"><topic id="6hhv3lsc3pn06bh78adhm0v5qa" structure-class="org.xmind.ui.map.unbalanced" timestamp="1571736575063"><title>cms数据库表</title><extensions><extension provider="org.xmind.ui.map.unbalanced"><content><right-number>0</right-number></content></extension></extensions><children><topics type="detached"><topic id="6q46gc9rln8fbpqabh5dptdi42" timestamp="1571735541238"><title>用户表</title><notes><html><xhtml:p>create table CMS_USER</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  USERCODE      VARCHAR2(50) not null,</xhtml:p><xhtml:p>  EMAIL         VARCHAR2(50),</xhtml:p><xhtml:p>  MOBILE        VARCHAR2(11),</xhtml:p><xhtml:p>  PASSWORD      VARCHAR2(40),</xhtml:p><xhtml:p>  NAME          VARCHAR2(50),</xhtml:p><xhtml:p>  GENDOR        VARCHAR2(2),</xhtml:p><xhtml:p>  BRANCH        VARCHAR2(20),</xhtml:p><xhtml:p>  DEPARTMENT    VARCHAR2(20),</xhtml:p><xhtml:p>  STATE         VARCHAR2(1),</xhtml:p><xhtml:p>  ADMINFLAG     VARCHAR2(1),</xhtml:p><xhtml:p>  PSWEXPIREDATE DATE,</xhtml:p><xhtml:p>  LASTLOGINDATE DATE,</xhtml:p><xhtml:p>  MAKEDATE      DATE,</xhtml:p><xhtml:p>  MAKEUSER      VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE    DATE,</xhtml:p><xhtml:p>  MODIFYUSER    VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p><xhtml:p/></html><plain>create table CMS_USER&#13;
(&#13;
  USERCODE      VARCHAR2(50) not null,&#13;
  EMAIL         VARCHAR2(50),&#13;
  MOBILE        VARCHAR2(11),&#13;
  PASSWORD      VARCHAR2(40),&#13;
  NAME          VARCHAR2(50),&#13;
  GENDOR        VARCHAR2(2),&#13;
  BRANCH        VARCHAR2(20),&#13;
  DEPARTMENT    VARCHAR2(20),&#13;
  STATE         VARCHAR2(1),&#13;
  ADMINFLAG     VARCHAR2(1),&#13;
  PSWEXPIREDATE DATE,&#13;
  LASTLOGINDATE DATE,&#13;
  MAKEDATE      DATE,&#13;
  MAKEUSER      VARCHAR2(20),&#13;
  MODIFYDATE    DATE,&#13;
  MODIFYUSER    VARCHAR2(20)&#13;
)&#13;
</plain></notes><position svg:x="263" svg:y="-132"/></topic><topic id="3mtoo3u6oe0vv0k4mdisd3rti3" timestamp="1571735651424"><title>角色表</title><position svg:x="267" svg:y="-70"/><notes><html><xhtml:p>create table CMS_ROLE</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  ROLEID     VARCHAR2(32) not null,</xhtml:p><xhtml:p>  ROLENAME   VARCHAR2(20),</xhtml:p><xhtml:p>  MAKEDATE   DATE,</xhtml:p><xhtml:p>  MAKEUSER   VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE DATE,</xhtml:p><xhtml:p>  MODIFYUSER VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CMS_ROLE&#13;
(&#13;
  ROLEID     VARCHAR2(32) not null,&#13;
  ROLENAME   VARCHAR2(20),&#13;
  MAKEDATE   DATE,&#13;
  MAKEUSER   VARCHAR2(20),&#13;
  MODIFYDATE DATE,&#13;
  MODIFYUSER VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="4sfvbl7h4udhi08cfu8rfsfafc" timestamp="1571735713904"><title>菜单表</title><position svg:x="268" svg:y="-1"/><notes><html><xhtml:p>create table CMS_MENU</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  MENUID       VARCHAR2(10) not null,</xhtml:p><xhtml:p>  MENUNAME     VARCHAR2(25),</xhtml:p><xhtml:p>  PARENTMENUID VARCHAR2(10),</xhtml:p><xhtml:p>  MENULINK     VARCHAR2(100),</xhtml:p><xhtml:p>  STATUS       VARCHAR2(1),</xhtml:p><xhtml:p>  NODEORDER    INTEGER,</xhtml:p><xhtml:p>  MAKEDATE     DATE,</xhtml:p><xhtml:p>  MAKEUSER     VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE   DATE,</xhtml:p><xhtml:p>  MODIFYUSER   VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CMS_MENU&#13;
(&#13;
  MENUID       VARCHAR2(10) not null,&#13;
  MENUNAME     VARCHAR2(25),&#13;
  PARENTMENUID VARCHAR2(10),&#13;
  MENULINK     VARCHAR2(100),&#13;
  STATUS       VARCHAR2(1),&#13;
  NODEORDER    INTEGER,&#13;
  MAKEDATE     DATE,&#13;
  MAKEUSER     VARCHAR2(20),&#13;
  MODIFYDATE   DATE,&#13;
  MODIFYUSER   VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="3oufor08h7f8j8seifpv1egpj9" timestamp="1571735806720"><title>用户角色关系表</title><position svg:x="310" svg:y="59"/><notes><html><xhtml:p>create table CMS_USERROLE</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  USERCODE   VARCHAR2(50) not null,</xhtml:p><xhtml:p>  ROLEID     VARCHAR2(32) not null,</xhtml:p><xhtml:p>  MAKEDATE   DATE,</xhtml:p><xhtml:p>  MAKEUSER   VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE DATE,</xhtml:p><xhtml:p>  MODIFYUSER VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CMS_USERROLE&#13;
(&#13;
  USERCODE   VARCHAR2(50) not null,&#13;
  ROLEID     VARCHAR2(32) not null,&#13;
  MAKEDATE   DATE,&#13;
  MAKEUSER   VARCHAR2(20),&#13;
  MODIFYDATE DATE,&#13;
  MODIFYUSER VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="69lsp702su58klccko1lnmik60" timestamp="1571735918753"><title>角色菜单表</title><position svg:x="289" svg:y="116"/><notes><html><xhtml:p>create table CMS_ROLEMENU</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  ROLEID     VARCHAR2(32) not null,</xhtml:p><xhtml:p>  ROLENAME   VARCHAR2(20),</xhtml:p><xhtml:p>  MENUID     VARCHAR2(200) not null,</xhtml:p><xhtml:p>  MAKEDATE   DATE,</xhtml:p><xhtml:p>  MAKEUSER   VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE DATE,</xhtml:p><xhtml:p>  MODIFYUSER VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CMS_ROLEMENU&#13;
(&#13;
  ROLEID     VARCHAR2(32) not null,&#13;
  ROLENAME   VARCHAR2(20),&#13;
  MENUID     VARCHAR2(200) not null,&#13;
  MAKEDATE   DATE,&#13;
  MAKEUSER   VARCHAR2(20),&#13;
  MODIFYDATE DATE,&#13;
  MODIFYUSER VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="0m67o7tm8a7n3tefj950c8n1oj" timestamp="1571735921984"><title>登录日志表</title><position svg:x="292" svg:y="172"/><notes><html><xhtml:p>create table CMS_LOGINTRACE</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  ID          VARCHAR2(32) not null,</xhtml:p><xhtml:p>  USERCODE    VARCHAR2(32),</xhtml:p><xhtml:p>  OPERATETYPE VARCHAR2(1),</xhtml:p><xhtml:p>  OPERATEDATE DATE,</xhtml:p><xhtml:p>  MAKEDATE    DATE,</xhtml:p><xhtml:p>  MAKEUSER    VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE  DATE,</xhtml:p><xhtml:p>  MODIFYUSER  VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CMS_LOGINTRACE&#13;
(&#13;
  ID          VARCHAR2(32) not null,&#13;
  USERCODE    VARCHAR2(32),&#13;
  OPERATETYPE VARCHAR2(1),&#13;
  OPERATEDATE DATE,&#13;
  MAKEDATE    DATE,&#13;
  MAKEUSER    VARCHAR2(20),&#13;
  MODIFYDATE  DATE,&#13;
  MODIFYUSER  VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="7v0a7b1ptmaqjtakce86hqvfln" timestamp="1571736394713"><title>批处理任务定义表</title><position svg:x="-428" svg:y="290"/><notes><html><xhtml:p>create table CF_JOBDEF</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  JOBCODE      VARCHAR2(6) not null,</xhtml:p><xhtml:p>  JOBNAME      VARCHAR2(80),</xhtml:p><xhtml:p>  JOBDESCRIBE  VARCHAR2(200),</xhtml:p><xhtml:p>  JOBCLASSNAME VARCHAR2(128),</xhtml:p><xhtml:p>  MAKEDATE     DATE,</xhtml:p><xhtml:p>  MAKEUSER     VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE   DATE,</xhtml:p><xhtml:p>  MODIFYUSER   VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CF_JOBDEF&#13;
(&#13;
  JOBCODE      VARCHAR2(6) not null,&#13;
  JOBNAME      VARCHAR2(80),&#13;
  JOBDESCRIBE  VARCHAR2(200),&#13;
  JOBCLASSNAME VARCHAR2(128),&#13;
  MAKEDATE     DATE,&#13;
  MAKEUSER     VARCHAR2(20),&#13;
  MODIFYDATE   DATE,&#13;
  MODIFYUSER   VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="24qb50bl747tmjse5q7k4873rq" timestamp="1571736396785"><title>批处理参数定义表</title><position svg:x="-427" svg:y="366"/><notes><html><xhtml:p>create table CF_JOBPARAMDEF</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  JOBCODE    VARCHAR2(6) not null,</xhtml:p><xhtml:p>  PARAMCODE  VARCHAR2(20) not null,</xhtml:p><xhtml:p>  PARAMNAME  VARCHAR2(20),</xhtml:p><xhtml:p>  MAKEDATE   DATE,</xhtml:p><xhtml:p>  MAKEUSER   VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE DATE,</xhtml:p><xhtml:p>  MODIFYUSER VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CF_JOBPARAMDEF&#13;
(&#13;
  JOBCODE    VARCHAR2(6) not null,&#13;
  PARAMCODE  VARCHAR2(20) not null,&#13;
  PARAMNAME  VARCHAR2(20),&#13;
  MAKEDATE   DATE,&#13;
  MAKEUSER   VARCHAR2(20),&#13;
  MODIFYDATE DATE,&#13;
  MODIFYUSER VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="3tvl56h17spi3urefud52b0e5g" timestamp="1571736398721"><title>批处理计划表</title><position svg:x="-451" svg:y="434"/><notes><html><xhtml:p>create table CF_JOBPLANDEF</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  JOBPLANCODE    VARCHAR2(32) not null,</xhtml:p><xhtml:p>  JOBCODE        VARCHAR2(6),</xhtml:p><xhtml:p>  JOBPLANDESC    VARCHAR2(200),</xhtml:p><xhtml:p>  RUNTYPE        VARCHAR2(5),</xhtml:p><xhtml:p>  CRONEXP        VARCHAR2(200),</xhtml:p><xhtml:p>  CRONEXPDESC    VARCHAR2(80),</xhtml:p><xhtml:p>  REPEATINTERVAL NUMBER(12),</xhtml:p><xhtml:p>  REPEATUNIT     VARCHAR2(2),</xhtml:p><xhtml:p>  STARTDATE      DATE,</xhtml:p><xhtml:p>  ENDDATE        DATE,</xhtml:p><xhtml:p>  USEFLAG        VARCHAR2(2),</xhtml:p><xhtml:p>  TRIGGERSTATE   VARCHAR2(2),</xhtml:p><xhtml:p>  MAKEDATE       DATE,</xhtml:p><xhtml:p>  MAKEUSER       VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE     DATE,</xhtml:p><xhtml:p>  MODIFYUSER     VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CF_JOBPLANDEF&#13;
(&#13;
  JOBPLANCODE    VARCHAR2(32) not null,&#13;
  JOBCODE        VARCHAR2(6),&#13;
  JOBPLANDESC    VARCHAR2(200),&#13;
  RUNTYPE        VARCHAR2(5),&#13;
  CRONEXP        VARCHAR2(200),&#13;
  CRONEXPDESC    VARCHAR2(80),&#13;
  REPEATINTERVAL NUMBER(12),&#13;
  REPEATUNIT     VARCHAR2(2),&#13;
  STARTDATE      DATE,&#13;
  ENDDATE        DATE,&#13;
  USEFLAG        VARCHAR2(2),&#13;
  TRIGGERSTATE   VARCHAR2(2),&#13;
  MAKEDATE       DATE,&#13;
  MAKEUSER       VARCHAR2(20),&#13;
  MODIFYDATE     DATE,&#13;
  MODIFYUSER     VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="05pq8if3jjjokn5n10jbeetmki" timestamp="1571736403305"><title>计划参数关系表</title><position svg:x="-438" svg:y="488"/><notes><html><xhtml:p>create table CF_JOBPLANPARAM</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  JOBCODE     VARCHAR2(6) not null,</xhtml:p><xhtml:p>  JOBPLANCODE VARCHAR2(32) not null,</xhtml:p><xhtml:p>  PARAMCODE   VARCHAR2(20) not null,</xhtml:p><xhtml:p>  PARAMVALUE  VARCHAR2(100),</xhtml:p><xhtml:p>  MAKEDATE    DATE,</xhtml:p><xhtml:p>  MAKEUSER    VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE  DATE,</xhtml:p><xhtml:p>  MODIFYUSER  VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CF_JOBPLANPARAM&#13;
(&#13;
  JOBCODE     VARCHAR2(6) not null,&#13;
  JOBPLANCODE VARCHAR2(32) not null,&#13;
  PARAMCODE   VARCHAR2(20) not null,&#13;
  PARAMVALUE  VARCHAR2(100),&#13;
  MAKEDATE    DATE,&#13;
  MAKEUSER    VARCHAR2(20),&#13;
  MODIFYDATE  DATE,&#13;
  MODIFYUSER  VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="4frmem76sg53mm1gbii2u8qird" timestamp="1571736402489"><title>计划运行日志表</title><position svg:x="-439" svg:y="554"/><notes><html><xhtml:p>create table CF_JOBRUNLOG</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  SERIALNO    VARCHAR2(20) not null,</xhtml:p><xhtml:p>  JOBCODE     VARCHAR2(6),</xhtml:p><xhtml:p>  JOBPLANCODE VARCHAR2(32),</xhtml:p><xhtml:p>  STARTDATE   DATE,</xhtml:p><xhtml:p>  ENDDATE     DATE,</xhtml:p><xhtml:p>  RUNSTATE    VARCHAR2(2),</xhtml:p><xhtml:p>  RUNRESULT   VARCHAR2(200),</xhtml:p><xhtml:p>  MAKEDATE    DATE,</xhtml:p><xhtml:p>  MAKEUSER    VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE  DATE,</xhtml:p><xhtml:p>  MODIFYUSER  VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CF_JOBRUNLOG&#13;
(&#13;
  SERIALNO    VARCHAR2(20) not null,&#13;
  JOBCODE     VARCHAR2(6),&#13;
  JOBPLANCODE VARCHAR2(32),&#13;
  STARTDATE   DATE,&#13;
  ENDDATE     DATE,&#13;
  RUNSTATE    VARCHAR2(2),&#13;
  RUNRESULT   VARCHAR2(200),&#13;
  MAKEDATE    DATE,&#13;
  MAKEUSER    VARCHAR2(20),&#13;
  MODIFYDATE  DATE,&#13;
  MODIFYUSER  VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="4f4bju806umt5qne93tdi484te" timestamp="1571736263022"><title>邮箱信息表</title><position svg:x="-417" svg:y="-3"/><notes><html><xhtml:p>create table CMS_EMAILMAININFO</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  ID         VARCHAR2(32) not null,</xhtml:p><xhtml:p>  EMAIL      VARCHAR2(50),</xhtml:p><xhtml:p>  EPASSWORD  VARCHAR2(20),</xhtml:p><xhtml:p>  EHOST      VARCHAR2(20),</xhtml:p><xhtml:p>  ENICKNAME  VARCHAR2(20),</xhtml:p><xhtml:p>  ESTATUS    VARCHAR2(2),</xhtml:p><xhtml:p>  EROLE      VARCHAR2(2),</xhtml:p><xhtml:p>  MAKEDATE   DATE,</xhtml:p><xhtml:p>  MAKEUSER   VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE DATE,</xhtml:p><xhtml:p>  MODIFYUSER VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CMS_EMAILMAININFO&#13;
(&#13;
  ID         VARCHAR2(32) not null,&#13;
  EMAIL      VARCHAR2(50),&#13;
  EPASSWORD  VARCHAR2(20),&#13;
  EHOST      VARCHAR2(20),&#13;
  ENICKNAME  VARCHAR2(20),&#13;
  ESTATUS    VARCHAR2(2),&#13;
  EROLE      VARCHAR2(2),&#13;
  MAKEDATE   DATE,&#13;
  MAKEUSER   VARCHAR2(20),&#13;
  MODIFYDATE DATE,&#13;
  MODIFYUSER VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="57vsu9shp983f18r94at3vqcjd" timestamp="1571736293104"><title>发送任务定义表</title><position svg:x="-408" svg:y="52"/><notes><html><xhtml:p>create table CMS_EMAILJOBDEF</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  EMAILJOBCODE     VARCHAR2(32) not null,</xhtml:p><xhtml:p>  EMAILJOBNAME     VARCHAR2(80),</xhtml:p><xhtml:p>  EMAILJOBDESCRIBE VARCHAR2(200),</xhtml:p><xhtml:p>  MAKEDATE         DATE,</xhtml:p><xhtml:p>  MAKEUSER         VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE       DATE,</xhtml:p><xhtml:p>  MODIFYUSER       VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CMS_EMAILJOBDEF&#13;
(&#13;
  EMAILJOBCODE     VARCHAR2(32) not null,&#13;
  EMAILJOBNAME     VARCHAR2(80),&#13;
  EMAILJOBDESCRIBE VARCHAR2(200),&#13;
  MAKEDATE         DATE,&#13;
  MAKEUSER         VARCHAR2(20),&#13;
  MODIFYDATE       DATE,&#13;
  MODIFYUSER       VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="59msg8vpm8phvpfai5ls0crf7q" timestamp="1571736333157"><title>发送任务邮箱关系表</title><position svg:x="-410" svg:y="114"/><notes><html><xhtml:p>create table CMS_EMAILJOBADDRESS</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  EMAILJOBCODE VARCHAR2(32) not null,</xhtml:p><xhtml:p>  EMAILID      VARCHAR2(80),</xhtml:p><xhtml:p>  EROLE        VARCHAR2(5),</xhtml:p><xhtml:p>  MAKEDATE     DATE,</xhtml:p><xhtml:p>  MAKEUSER     VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE   DATE,</xhtml:p><xhtml:p>  MODIFYUSER   VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CMS_EMAILJOBADDRESS&#13;
(&#13;
  EMAILJOBCODE VARCHAR2(32) not null,&#13;
  EMAILID      VARCHAR2(80),&#13;
  EROLE        VARCHAR2(5),&#13;
  MAKEDATE     DATE,&#13;
  MAKEUSER     VARCHAR2(20),&#13;
  MODIFYDATE   DATE,&#13;
  MODIFYUSER   VARCHAR2(20)&#13;
)</plain></notes></topic></topics></children><marker-refs><marker-ref marker-id="smiley-boring"/></marker-refs></topic><title>画布 1</title><relationships><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="6q46gc9rln8fbpqabh5dptdi42" id="6j4u1pmsb9uo2897gb5pd62fjr" timestamp="1571735389949"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="3mtoo3u6oe0vv0k4mdisd3rti3" id="5lemqinckf726jg3os7bkgkin1" timestamp="1571735551450"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="4sfvbl7h4udhi08cfu8rfsfafc" id="0o5t7rr00raoh9lthllrosh9qi" timestamp="1571735693147"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="3oufor08h7f8j8seifpv1egpj9" id="2uptojutqb7l3ddr2gpo936vhp" timestamp="1571735763609"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="4f4bju806umt5qne93tdi484te" id="4eg7u7llsb050btgvd5m6i03fp" timestamp="1571736341449"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="57vsu9shp983f18r94at3vqcjd" id="75n50ugjf31ujkh4d62th72q6s" timestamp="1571736347321"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="59msg8vpm8phvpfai5ls0crf7q" id="61ccca5lgrctsrvht8hk9j2jnk" timestamp="1571736362161"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="7v0a7b1ptmaqjtakce86hqvfln" id="6he84jgb7caqflhgge5bv2scjf" timestamp="1571736370889"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="24qb50bl747tmjse5q7k4873rq" id="57qbo3cpd8d1ct04vp0o4537no" timestamp="1571736376209"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="3tvl56h17spi3urefud52b0e5g" id="34hvqiv410hpbavvq4ui3mtgfc" timestamp="1571736382185"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="05pq8if3jjjokn5n10jbeetmki" id="38vs6intq1m45rrfdrdk8dtck3" timestamp="1571736386801"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="4frmem76sg53mm1gbii2u8qird" id="2kqdj9san7ulh0a2no39rsb425" timestamp="1571736391722"/></relationships></sheet></xmap-content>PK<ӵ,
C  C  PK  ��VO            
   styles.xml��<?xml version="1.0" encoding="UTF-8" standalone="no"?><xmap-styles xmlns="urn:xmind:xmap:xmlns:style:2.0" xmlns:fo="http://www.w3.org/1999/XSL/Format" xmlns:svg="http://www.w3.org/2000/svg" version="2.0"><automatic-styles><style id="2ci8evjkhmr5m5tkgafaumb35m" name="" type="relationship">
			<relationship-properties arrow-begin-class="org.xmind.arrowShape.none" arrow-end-class="org.xmind.arrowShape.triangle" fo:color="#BF1E1B" fo:font-family="Comic Sans MS" fo:font-size="12pt" line-color="#BF1E1B" line-pattern="dash" line-width="1pt" shape-class="org.xmind.relationshipShape.curved"/>
		</style><style id="20imgh8165s0ch5i3r71bde560" name="" type="topic">
			<topic-properties fo:color="#004080" fo:font-family="Verdana" fo:font-weight="normal" line-class="org.xmind.branchConnection.curve" line-color="#004080" shape-class="org.xmind.topicShape.roundedRect" svg:fill="#68A3DF"/>
		</style><style id="3a9i9g231bi15sjip958ldvc2a" name="" type="topic">
			<topic-properties fo:color="#004080" fo:font-family="Verdana" svg:fill="none"/>
		</style><style id="1meu19hsvqff5e9aeeulslcega" name="" type="topic">
			<topic-properties fo:color="#004080" fo:font-family="Verdana" fo:font-weight="normal" line-class="org.xmind.branchConnection.curve" line-color="#004080" shape-class="org.xmind.topicShape.roundedRect" svg:fill="#D3DFFF"/>
		</style><style id="6haq0nnra20q2d6kq7pe4e8168" name="" type="topic">
			<topic-properties fo:color="#004080" fo:font-family="Verdana" svg:fill="#D3DFFF"/>
		</style><style id="7ba0jerumtm0ngq12oc01p3iih" name="" type="topic">
			<topic-properties border-line-width="0pt" fo:color="#BF1E1B" fo:font-family="Comic Sans MS" fo:font-size="12pt" line-class="org.xmind.branchConnection.arrowedCurve" shape-class="org.xmind.topicShape.ellipse" svg:fill="none"/>
		</style><style id="2fcia2jt9sobnapjdplqqkuusq" name="" type="boundary">
			<boundary-properties fo:color="#535353" fo:font-family="Verdana" line-color="#999999" line-pattern="dash" line-width="1pt" shape-class="org.xmind.boundaryShape.scallops" svg:fill="#FFFFFF"/>
		</style></automatic-styles><master-styles><style id="xminddefaultthemeid2014" name="%professional" type="theme">
			<theme-properties>
				<default-style style-family="relationship" style-id="2ci8evjkhmr5m5tkgafaumb35m"/>
				<default-style style-family="centralTopic" style-id="20imgh8165s0ch5i3r71bde560"/>
				<default-style style-family="subTopic" style-id="3a9i9g231bi15sjip958ldvc2a"/>
				<default-style style-family="floatingTopic" style-id="1meu19hsvqff5e9aeeulslcega"/>
				<default-style style-family="mainTopic" style-id="6haq0nnra20q2d6kq7pe4e8168"/>
				<default-style style-family="summaryTopic" style-id="7ba0jerumtm0ngq12oc01p3iih"/>
				<default-style style-family="boundary" style-id="2fcia2jt9sobnapjdplqqkuusq"/>
			</theme-properties>
		</style></master-styles><styles><style id="3b7n6l540kiaagavceovs7toh1" type="map"><map-properties color-gradient="gradient" line-tapered="tapered" multi-line-colors="#ac6060 #acac60 #60ac60 #60acac #6060ac #ac60ac"/></style></styles></xmap-styles>PK�0��    PK  ��VO            2   Revisions/4c8cdrtv5uli10r8nr70grk327/revisions.xml ��<?xml version="1.0" encoding="UTF-8" standalone="no"?><xmap-revisions media-type="application/vnd.xmind.sheet" next-rev-num="3" resource-id="4c8cdrtv5uli10r8nr70grk327"><revision creator-name="XMind" creator-version="3.5.1.201411201906" resource="Revisions/4c8cdrtv5uli10r8nr70grk327/rev-1-1571736424210.xml" rev-num="1" timestamp="1571736424210"/><revision creator-name="XMind" creator-version="3.5.1.201411201906" resource="Revisions/4c8cdrtv5uli10r8nr70grk327/rev-2-1571736578774.xml" rev-num="2" timestamp="1571736578774"/></xmap-revisions>PK��Q%     PK  ��VO            <   Revisions/4c8cdrtv5uli10r8nr70grk327/rev-1-1571736424210.xml�B�<?xml version="1.0" encoding="UTF-8" standalone="no"?><xmap-revision-content xmlns="urn:xmind:xmap:xmlns:revision:1.0" xmlns:fo="http://www.w3.org/1999/XSL/Format" xmlns:svg="http://www.w3.org/2000/svg" xmlns:xhtml="http://www.w3.org/1999/xhtml" xmlns:xlink="http://www.w3.org/1999/xlink"><sheet id="4c8cdrtv5uli10r8nr70grk327" style-id="3b7n6l540kiaagavceovs7toh1" theme="xminddefaultthemeid2014" timestamp="1571736403305"><topic id="6hhv3lsc3pn06bh78adhm0v5qa" structure-class="org.xmind.ui.map.unbalanced" timestamp="1571736403305"><title>cms数据库表</title><marker-refs><marker-ref marker-id="smiley-smile"/></marker-refs><extensions><extension provider="org.xmind.ui.map.unbalanced"><content><right-number>0</right-number></content></extension></extensions><children><topics type="detached"><topic id="6q46gc9rln8fbpqabh5dptdi42" timestamp="1571735541238"><title>用户表</title><notes><html><xhtml:p>create table CMS_USER</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  USERCODE      VARCHAR2(50) not null,</xhtml:p><xhtml:p>  EMAIL         VARCHAR2(50),</xhtml:p><xhtml:p>  MOBILE        VARCHAR2(11),</xhtml:p><xhtml:p>  PASSWORD      VARCHAR2(40),</xhtml:p><xhtml:p>  NAME          VARCHAR2(50),</xhtml:p><xhtml:p>  GENDOR        VARCHAR2(2),</xhtml:p><xhtml:p>  BRANCH        VARCHAR2(20),</xhtml:p><xhtml:p>  DEPARTMENT    VARCHAR2(20),</xhtml:p><xhtml:p>  STATE         VARCHAR2(1),</xhtml:p><xhtml:p>  ADMINFLAG     VARCHAR2(1),</xhtml:p><xhtml:p>  PSWEXPIREDATE DATE,</xhtml:p><xhtml:p>  LASTLOGINDATE DATE,</xhtml:p><xhtml:p>  MAKEDATE      DATE,</xhtml:p><xhtml:p>  MAKEUSER      VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE    DATE,</xhtml:p><xhtml:p>  MODIFYUSER    VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p><xhtml:p/></html><plain>create table CMS_USER&#13;
(&#13;
  USERCODE      VARCHAR2(50) not null,&#13;
  EMAIL         VARCHAR2(50),&#13;
  MOBILE        VARCHAR2(11),&#13;
  PASSWORD      VARCHAR2(40),&#13;
  NAME          VARCHAR2(50),&#13;
  GENDOR        VARCHAR2(2),&#13;
  BRANCH        VARCHAR2(20),&#13;
  DEPARTMENT    VARCHAR2(20),&#13;
  STATE         VARCHAR2(1),&#13;
  ADMINFLAG     VARCHAR2(1),&#13;
  PSWEXPIREDATE DATE,&#13;
  LASTLOGINDATE DATE,&#13;
  MAKEDATE      DATE,&#13;
  MAKEUSER      VARCHAR2(20),&#13;
  MODIFYDATE    DATE,&#13;
  MODIFYUSER    VARCHAR2(20)&#13;
)&#13;
</plain></notes><position svg:x="263" svg:y="-132"/></topic><topic id="3mtoo3u6oe0vv0k4mdisd3rti3" timestamp="1571735651424"><title>角色表</title><position svg:x="267" svg:y="-70"/><notes><html><xhtml:p>create table CMS_ROLE</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  ROLEID     VARCHAR2(32) not null,</xhtml:p><xhtml:p>  ROLENAME   VARCHAR2(20),</xhtml:p><xhtml:p>  MAKEDATE   DATE,</xhtml:p><xhtml:p>  MAKEUSER   VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE DATE,</xhtml:p><xhtml:p>  MODIFYUSER VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CMS_ROLE&#13;
(&#13;
  ROLEID     VARCHAR2(32) not null,&#13;
  ROLENAME   VARCHAR2(20),&#13;
  MAKEDATE   DATE,&#13;
  MAKEUSER   VARCHAR2(20),&#13;
  MODIFYDATE DATE,&#13;
  MODIFYUSER VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="4sfvbl7h4udhi08cfu8rfsfafc" timestamp="1571735713904"><title>菜单表</title><position svg:x="268" svg:y="-1"/><notes><html><xhtml:p>create table CMS_MENU</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  MENUID       VARCHAR2(10) not null,</xhtml:p><xhtml:p>  MENUNAME     VARCHAR2(25),</xhtml:p><xhtml:p>  PARENTMENUID VARCHAR2(10),</xhtml:p><xhtml:p>  MENULINK     VARCHAR2(100),</xhtml:p><xhtml:p>  STATUS       VARCHAR2(1),</xhtml:p><xhtml:p>  NODEORDER    INTEGER,</xhtml:p><xhtml:p>  MAKEDATE     DATE,</xhtml:p><xhtml:p>  MAKEUSER     VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE   DATE,</xhtml:p><xhtml:p>  MODIFYUSER   VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CMS_MENU&#13;
(&#13;
  MENUID       VARCHAR2(10) not null,&#13;
  MENUNAME     VARCHAR2(25),&#13;
  PARENTMENUID VARCHAR2(10),&#13;
  MENULINK     VARCHAR2(100),&#13;
  STATUS       VARCHAR2(1),&#13;
  NODEORDER    INTEGER,&#13;
  MAKEDATE     DATE,&#13;
  MAKEUSER     VARCHAR2(20),&#13;
  MODIFYDATE   DATE,&#13;
  MODIFYUSER   VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="3oufor08h7f8j8seifpv1egpj9" timestamp="1571735806720"><title>用户角色关系表</title><position svg:x="310" svg:y="59"/><notes><html><xhtml:p>create table CMS_USERROLE</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  USERCODE   VARCHAR2(50) not null,</xhtml:p><xhtml:p>  ROLEID     VARCHAR2(32) not null,</xhtml:p><xhtml:p>  MAKEDATE   DATE,</xhtml:p><xhtml:p>  MAKEUSER   VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE DATE,</xhtml:p><xhtml:p>  MODIFYUSER VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CMS_USERROLE&#13;
(&#13;
  USERCODE   VARCHAR2(50) not null,&#13;
  ROLEID     VARCHAR2(32) not null,&#13;
  MAKEDATE   DATE,&#13;
  MAKEUSER   VARCHAR2(20),&#13;
  MODIFYDATE DATE,&#13;
  MODIFYUSER VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="69lsp702su58klccko1lnmik60" timestamp="1571735918753"><title>角色菜单表</title><position svg:x="289" svg:y="116"/><notes><html><xhtml:p>create table CMS_ROLEMENU</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  ROLEID     VARCHAR2(32) not null,</xhtml:p><xhtml:p>  ROLENAME   VARCHAR2(20),</xhtml:p><xhtml:p>  MENUID     VARCHAR2(200) not null,</xhtml:p><xhtml:p>  MAKEDATE   DATE,</xhtml:p><xhtml:p>  MAKEUSER   VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE DATE,</xhtml:p><xhtml:p>  MODIFYUSER VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CMS_ROLEMENU&#13;
(&#13;
  ROLEID     VARCHAR2(32) not null,&#13;
  ROLENAME   VARCHAR2(20),&#13;
  MENUID     VARCHAR2(200) not null,&#13;
  MAKEDATE   DATE,&#13;
  MAKEUSER   VARCHAR2(20),&#13;
  MODIFYDATE DATE,&#13;
  MODIFYUSER VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="0m67o7tm8a7n3tefj950c8n1oj" timestamp="1571735921984"><title>登录日志表</title><position svg:x="292" svg:y="172"/><notes><html><xhtml:p>create table CMS_LOGINTRACE</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  ID          VARCHAR2(32) not null,</xhtml:p><xhtml:p>  USERCODE    VARCHAR2(32),</xhtml:p><xhtml:p>  OPERATETYPE VARCHAR2(1),</xhtml:p><xhtml:p>  OPERATEDATE DATE,</xhtml:p><xhtml:p>  MAKEDATE    DATE,</xhtml:p><xhtml:p>  MAKEUSER    VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE  DATE,</xhtml:p><xhtml:p>  MODIFYUSER  VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CMS_LOGINTRACE&#13;
(&#13;
  ID          VARCHAR2(32) not null,&#13;
  USERCODE    VARCHAR2(32),&#13;
  OPERATETYPE VARCHAR2(1),&#13;
  OPERATEDATE DATE,&#13;
  MAKEDATE    DATE,&#13;
  MAKEUSER    VARCHAR2(20),&#13;
  MODIFYDATE  DATE,&#13;
  MODIFYUSER  VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="7v0a7b1ptmaqjtakce86hqvfln" timestamp="1571736394713"><title>批处理任务定义表</title><position svg:x="-428" svg:y="290"/><notes><html><xhtml:p>create table CF_JOBDEF</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  JOBCODE      VARCHAR2(6) not null,</xhtml:p><xhtml:p>  JOBNAME      VARCHAR2(80),</xhtml:p><xhtml:p>  JOBDESCRIBE  VARCHAR2(200),</xhtml:p><xhtml:p>  JOBCLASSNAME VARCHAR2(128),</xhtml:p><xhtml:p>  MAKEDATE     DATE,</xhtml:p><xhtml:p>  MAKEUSER     VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE   DATE,</xhtml:p><xhtml:p>  MODIFYUSER   VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CF_JOBDEF&#13;
(&#13;
  JOBCODE      VARCHAR2(6) not null,&#13;
  JOBNAME      VARCHAR2(80),&#13;
  JOBDESCRIBE  VARCHAR2(200),&#13;
  JOBCLASSNAME VARCHAR2(128),&#13;
  MAKEDATE     DATE,&#13;
  MAKEUSER     VARCHAR2(20),&#13;
  MODIFYDATE   DATE,&#13;
  MODIFYUSER   VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="24qb50bl747tmjse5q7k4873rq" timestamp="1571736396785"><title>批处理参数定义表</title><position svg:x="-427" svg:y="366"/><notes><html><xhtml:p>create table CF_JOBPARAMDEF</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  JOBCODE    VARCHAR2(6) not null,</xhtml:p><xhtml:p>  PARAMCODE  VARCHAR2(20) not null,</xhtml:p><xhtml:p>  PARAMNAME  VARCHAR2(20),</xhtml:p><xhtml:p>  MAKEDATE   DATE,</xhtml:p><xhtml:p>  MAKEUSER   VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE DATE,</xhtml:p><xhtml:p>  MODIFYUSER VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CF_JOBPARAMDEF&#13;
(&#13;
  JOBCODE    VARCHAR2(6) not null,&#13;
  PARAMCODE  VARCHAR2(20) not null,&#13;
  PARAMNAME  VARCHAR2(20),&#13;
  MAKEDATE   DATE,&#13;
  MAKEUSER   VARCHAR2(20),&#13;
  MODIFYDATE DATE,&#13;
  MODIFYUSER VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="3tvl56h17spi3urefud52b0e5g" timestamp="1571736398721"><title>批处理计划表</title><position svg:x="-451" svg:y="434"/><notes><html><xhtml:p>create table CF_JOBPLANDEF</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  JOBPLANCODE    VARCHAR2(32) not null,</xhtml:p><xhtml:p>  JOBCODE        VARCHAR2(6),</xhtml:p><xhtml:p>  JOBPLANDESC    VARCHAR2(200),</xhtml:p><xhtml:p>  RUNTYPE        VARCHAR2(5),</xhtml:p><xhtml:p>  CRONEXP        VARCHAR2(200),</xhtml:p><xhtml:p>  CRONEXPDESC    VARCHAR2(80),</xhtml:p><xhtml:p>  REPEATINTERVAL NUMBER(12),</xhtml:p><xhtml:p>  REPEATUNIT     VARCHAR2(2),</xhtml:p><xhtml:p>  STARTDATE      DATE,</xhtml:p><xhtml:p>  ENDDATE        DATE,</xhtml:p><xhtml:p>  USEFLAG        VARCHAR2(2),</xhtml:p><xhtml:p>  TRIGGERSTATE   VARCHAR2(2),</xhtml:p><xhtml:p>  MAKEDATE       DATE,</xhtml:p><xhtml:p>  MAKEUSER       VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE     DATE,</xhtml:p><xhtml:p>  MODIFYUSER     VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CF_JOBPLANDEF&#13;
(&#13;
  JOBPLANCODE    VARCHAR2(32) not null,&#13;
  JOBCODE        VARCHAR2(6),&#13;
  JOBPLANDESC    VARCHAR2(200),&#13;
  RUNTYPE        VARCHAR2(5),&#13;
  CRONEXP        VARCHAR2(200),&#13;
  CRONEXPDESC    VARCHAR2(80),&#13;
  REPEATINTERVAL NUMBER(12),&#13;
  REPEATUNIT     VARCHAR2(2),&#13;
  STARTDATE      DATE,&#13;
  ENDDATE        DATE,&#13;
  USEFLAG        VARCHAR2(2),&#13;
  TRIGGERSTATE   VARCHAR2(2),&#13;
  MAKEDATE       DATE,&#13;
  MAKEUSER       VARCHAR2(20),&#13;
  MODIFYDATE     DATE,&#13;
  MODIFYUSER     VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="05pq8if3jjjokn5n10jbeetmki" timestamp="1571736403305"><title>计划参数关系表</title><position svg:x="-438" svg:y="488"/><notes><html><xhtml:p>create table CF_JOBPLANPARAM</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  JOBCODE     VARCHAR2(6) not null,</xhtml:p><xhtml:p>  JOBPLANCODE VARCHAR2(32) not null,</xhtml:p><xhtml:p>  PARAMCODE   VARCHAR2(20) not null,</xhtml:p><xhtml:p>  PARAMVALUE  VARCHAR2(100),</xhtml:p><xhtml:p>  MAKEDATE    DATE,</xhtml:p><xhtml:p>  MAKEUSER    VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE  DATE,</xhtml:p><xhtml:p>  MODIFYUSER  VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CF_JOBPLANPARAM&#13;
(&#13;
  JOBCODE     VARCHAR2(6) not null,&#13;
  JOBPLANCODE VARCHAR2(32) not null,&#13;
  PARAMCODE   VARCHAR2(20) not null,&#13;
  PARAMVALUE  VARCHAR2(100),&#13;
  MAKEDATE    DATE,&#13;
  MAKEUSER    VARCHAR2(20),&#13;
  MODIFYDATE  DATE,&#13;
  MODIFYUSER  VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="4frmem76sg53mm1gbii2u8qird" timestamp="1571736402489"><title>计划运行日志表</title><position svg:x="-439" svg:y="554"/><notes><html><xhtml:p>create table CF_JOBRUNLOG</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  SERIALNO    VARCHAR2(20) not null,</xhtml:p><xhtml:p>  JOBCODE     VARCHAR2(6),</xhtml:p><xhtml:p>  JOBPLANCODE VARCHAR2(32),</xhtml:p><xhtml:p>  STARTDATE   DATE,</xhtml:p><xhtml:p>  ENDDATE     DATE,</xhtml:p><xhtml:p>  RUNSTATE    VARCHAR2(2),</xhtml:p><xhtml:p>  RUNRESULT   VARCHAR2(200),</xhtml:p><xhtml:p>  MAKEDATE    DATE,</xhtml:p><xhtml:p>  MAKEUSER    VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE  DATE,</xhtml:p><xhtml:p>  MODIFYUSER  VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CF_JOBRUNLOG&#13;
(&#13;
  SERIALNO    VARCHAR2(20) not null,&#13;
  JOBCODE     VARCHAR2(6),&#13;
  JOBPLANCODE VARCHAR2(32),&#13;
  STARTDATE   DATE,&#13;
  ENDDATE     DATE,&#13;
  RUNSTATE    VARCHAR2(2),&#13;
  RUNRESULT   VARCHAR2(200),&#13;
  MAKEDATE    DATE,&#13;
  MAKEUSER    VARCHAR2(20),&#13;
  MODIFYDATE  DATE,&#13;
  MODIFYUSER  VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="4f4bju806umt5qne93tdi484te" timestamp="1571736263022"><title>邮箱信息表</title><position svg:x="-417" svg:y="-3"/><notes><html><xhtml:p>create table CMS_EMAILMAININFO</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  ID         VARCHAR2(32) not null,</xhtml:p><xhtml:p>  EMAIL      VARCHAR2(50),</xhtml:p><xhtml:p>  EPASSWORD  VARCHAR2(20),</xhtml:p><xhtml:p>  EHOST      VARCHAR2(20),</xhtml:p><xhtml:p>  ENICKNAME  VARCHAR2(20),</xhtml:p><xhtml:p>  ESTATUS    VARCHAR2(2),</xhtml:p><xhtml:p>  EROLE      VARCHAR2(2),</xhtml:p><xhtml:p>  MAKEDATE   DATE,</xhtml:p><xhtml:p>  MAKEUSER   VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE DATE,</xhtml:p><xhtml:p>  MODIFYUSER VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CMS_EMAILMAININFO&#13;
(&#13;
  ID         VARCHAR2(32) not null,&#13;
  EMAIL      VARCHAR2(50),&#13;
  EPASSWORD  VARCHAR2(20),&#13;
  EHOST      VARCHAR2(20),&#13;
  ENICKNAME  VARCHAR2(20),&#13;
  ESTATUS    VARCHAR2(2),&#13;
  EROLE      VARCHAR2(2),&#13;
  MAKEDATE   DATE,&#13;
  MAKEUSER   VARCHAR2(20),&#13;
  MODIFYDATE DATE,&#13;
  MODIFYUSER VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="57vsu9shp983f18r94at3vqcjd" timestamp="1571736293104"><title>发送任务定义表</title><position svg:x="-408" svg:y="52"/><notes><html><xhtml:p>create table CMS_EMAILJOBDEF</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  EMAILJOBCODE     VARCHAR2(32) not null,</xhtml:p><xhtml:p>  EMAILJOBNAME     VARCHAR2(80),</xhtml:p><xhtml:p>  EMAILJOBDESCRIBE VARCHAR2(200),</xhtml:p><xhtml:p>  MAKEDATE         DATE,</xhtml:p><xhtml:p>  MAKEUSER         VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE       DATE,</xhtml:p><xhtml:p>  MODIFYUSER       VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CMS_EMAILJOBDEF&#13;
(&#13;
  EMAILJOBCODE     VARCHAR2(32) not null,&#13;
  EMAILJOBNAME     VARCHAR2(80),&#13;
  EMAILJOBDESCRIBE VARCHAR2(200),&#13;
  MAKEDATE         DATE,&#13;
  MAKEUSER         VARCHAR2(20),&#13;
  MODIFYDATE       DATE,&#13;
  MODIFYUSER       VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="59msg8vpm8phvpfai5ls0crf7q" timestamp="1571736333157"><title>发送任务邮箱关系表</title><position svg:x="-410" svg:y="114"/><notes><html><xhtml:p>create table CMS_EMAILJOBADDRESS</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  EMAILJOBCODE VARCHAR2(32) not null,</xhtml:p><xhtml:p>  EMAILID      VARCHAR2(80),</xhtml:p><xhtml:p>  EROLE        VARCHAR2(5),</xhtml:p><xhtml:p>  MAKEDATE     DATE,</xhtml:p><xhtml:p>  MAKEUSER     VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE   DATE,</xhtml:p><xhtml:p>  MODIFYUSER   VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CMS_EMAILJOBADDRESS&#13;
(&#13;
  EMAILJOBCODE VARCHAR2(32) not null,&#13;
  EMAILID      VARCHAR2(80),&#13;
  EROLE        VARCHAR2(5),&#13;
  MAKEDATE     DATE,&#13;
  MAKEUSER     VARCHAR2(20),&#13;
  MODIFYDATE   DATE,&#13;
  MODIFYUSER   VARCHAR2(20)&#13;
)</plain></notes></topic></topics></children></topic><title>画布 1</title><relationships><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="6q46gc9rln8fbpqabh5dptdi42" id="6j4u1pmsb9uo2897gb5pd62fjr" timestamp="1571735389949"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="3mtoo3u6oe0vv0k4mdisd3rti3" id="5lemqinckf726jg3os7bkgkin1" timestamp="1571735551450"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="4sfvbl7h4udhi08cfu8rfsfafc" id="0o5t7rr00raoh9lthllrosh9qi" timestamp="1571735693147"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="3oufor08h7f8j8seifpv1egpj9" id="2uptojutqb7l3ddr2gpo936vhp" timestamp="1571735763609"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="4f4bju806umt5qne93tdi484te" id="4eg7u7llsb050btgvd5m6i03fp" timestamp="1571736341449"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="57vsu9shp983f18r94at3vqcjd" id="75n50ugjf31ujkh4d62th72q6s" timestamp="1571736347321"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="59msg8vpm8phvpfai5ls0crf7q" id="61ccca5lgrctsrvht8hk9j2jnk" timestamp="1571736362161"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="7v0a7b1ptmaqjtakce86hqvfln" id="6he84jgb7caqflhgge5bv2scjf" timestamp="1571736370889"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="24qb50bl747tmjse5q7k4873rq" id="57qbo3cpd8d1ct04vp0o4537no" timestamp="1571736376209"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="3tvl56h17spi3urefud52b0e5g" id="34hvqiv410hpbavvq4ui3mtgfc" timestamp="1571736382185"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="05pq8if3jjjokn5n10jbeetmki" id="38vs6intq1m45rrfdrdk8dtck3" timestamp="1571736386801"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="4frmem76sg53mm1gbii2u8qird" id="2kqdj9san7ulh0a2no39rsb425" timestamp="1571736391722"/></relationships></sheet></xmap-revision-content>PKuWTq�B  �B  PK  ��VO            <   Revisions/4c8cdrtv5uli10r8nr70grk327/rev-2-1571736578774.xmlC�<?xml version="1.0" encoding="UTF-8" standalone="no"?><xmap-revision-content xmlns="urn:xmind:xmap:xmlns:revision:1.0" xmlns:fo="http://www.w3.org/1999/XSL/Format" xmlns:svg="http://www.w3.org/2000/svg" xmlns:xhtml="http://www.w3.org/1999/xhtml" xmlns:xlink="http://www.w3.org/1999/xlink"><sheet id="4c8cdrtv5uli10r8nr70grk327" style-id="3b7n6l540kiaagavceovs7toh1" theme="xminddefaultthemeid2014" timestamp="1571736575064" xmlns="urn:xmind:xmap:xmlns:content:2.0"><topic id="6hhv3lsc3pn06bh78adhm0v5qa" structure-class="org.xmind.ui.map.unbalanced" timestamp="1571736575063"><title>cms数据库表</title><extensions><extension provider="org.xmind.ui.map.unbalanced"><content><right-number>0</right-number></content></extension></extensions><children><topics type="detached"><topic id="6q46gc9rln8fbpqabh5dptdi42" timestamp="1571735541238"><title>用户表</title><notes><html><xhtml:p>create table CMS_USER</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  USERCODE      VARCHAR2(50) not null,</xhtml:p><xhtml:p>  EMAIL         VARCHAR2(50),</xhtml:p><xhtml:p>  MOBILE        VARCHAR2(11),</xhtml:p><xhtml:p>  PASSWORD      VARCHAR2(40),</xhtml:p><xhtml:p>  NAME          VARCHAR2(50),</xhtml:p><xhtml:p>  GENDOR        VARCHAR2(2),</xhtml:p><xhtml:p>  BRANCH        VARCHAR2(20),</xhtml:p><xhtml:p>  DEPARTMENT    VARCHAR2(20),</xhtml:p><xhtml:p>  STATE         VARCHAR2(1),</xhtml:p><xhtml:p>  ADMINFLAG     VARCHAR2(1),</xhtml:p><xhtml:p>  PSWEXPIREDATE DATE,</xhtml:p><xhtml:p>  LASTLOGINDATE DATE,</xhtml:p><xhtml:p>  MAKEDATE      DATE,</xhtml:p><xhtml:p>  MAKEUSER      VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE    DATE,</xhtml:p><xhtml:p>  MODIFYUSER    VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p><xhtml:p/></html><plain>create table CMS_USER&#13;
(&#13;
  USERCODE      VARCHAR2(50) not null,&#13;
  EMAIL         VARCHAR2(50),&#13;
  MOBILE        VARCHAR2(11),&#13;
  PASSWORD      VARCHAR2(40),&#13;
  NAME          VARCHAR2(50),&#13;
  GENDOR        VARCHAR2(2),&#13;
  BRANCH        VARCHAR2(20),&#13;
  DEPARTMENT    VARCHAR2(20),&#13;
  STATE         VARCHAR2(1),&#13;
  ADMINFLAG     VARCHAR2(1),&#13;
  PSWEXPIREDATE DATE,&#13;
  LASTLOGINDATE DATE,&#13;
  MAKEDATE      DATE,&#13;
  MAKEUSER      VARCHAR2(20),&#13;
  MODIFYDATE    DATE,&#13;
  MODIFYUSER    VARCHAR2(20)&#13;
)&#13;
</plain></notes><position svg:x="263" svg:y="-132"/></topic><topic id="3mtoo3u6oe0vv0k4mdisd3rti3" timestamp="1571735651424"><title>角色表</title><position svg:x="267" svg:y="-70"/><notes><html><xhtml:p>create table CMS_ROLE</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  ROLEID     VARCHAR2(32) not null,</xhtml:p><xhtml:p>  ROLENAME   VARCHAR2(20),</xhtml:p><xhtml:p>  MAKEDATE   DATE,</xhtml:p><xhtml:p>  MAKEUSER   VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE DATE,</xhtml:p><xhtml:p>  MODIFYUSER VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CMS_ROLE&#13;
(&#13;
  ROLEID     VARCHAR2(32) not null,&#13;
  ROLENAME   VARCHAR2(20),&#13;
  MAKEDATE   DATE,&#13;
  MAKEUSER   VARCHAR2(20),&#13;
  MODIFYDATE DATE,&#13;
  MODIFYUSER VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="4sfvbl7h4udhi08cfu8rfsfafc" timestamp="1571735713904"><title>菜单表</title><position svg:x="268" svg:y="-1"/><notes><html><xhtml:p>create table CMS_MENU</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  MENUID       VARCHAR2(10) not null,</xhtml:p><xhtml:p>  MENUNAME     VARCHAR2(25),</xhtml:p><xhtml:p>  PARENTMENUID VARCHAR2(10),</xhtml:p><xhtml:p>  MENULINK     VARCHAR2(100),</xhtml:p><xhtml:p>  STATUS       VARCHAR2(1),</xhtml:p><xhtml:p>  NODEORDER    INTEGER,</xhtml:p><xhtml:p>  MAKEDATE     DATE,</xhtml:p><xhtml:p>  MAKEUSER     VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE   DATE,</xhtml:p><xhtml:p>  MODIFYUSER   VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CMS_MENU&#13;
(&#13;
  MENUID       VARCHAR2(10) not null,&#13;
  MENUNAME     VARCHAR2(25),&#13;
  PARENTMENUID VARCHAR2(10),&#13;
  MENULINK     VARCHAR2(100),&#13;
  STATUS       VARCHAR2(1),&#13;
  NODEORDER    INTEGER,&#13;
  MAKEDATE     DATE,&#13;
  MAKEUSER     VARCHAR2(20),&#13;
  MODIFYDATE   DATE,&#13;
  MODIFYUSER   VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="3oufor08h7f8j8seifpv1egpj9" timestamp="1571735806720"><title>用户角色关系表</title><position svg:x="310" svg:y="59"/><notes><html><xhtml:p>create table CMS_USERROLE</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  USERCODE   VARCHAR2(50) not null,</xhtml:p><xhtml:p>  ROLEID     VARCHAR2(32) not null,</xhtml:p><xhtml:p>  MAKEDATE   DATE,</xhtml:p><xhtml:p>  MAKEUSER   VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE DATE,</xhtml:p><xhtml:p>  MODIFYUSER VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CMS_USERROLE&#13;
(&#13;
  USERCODE   VARCHAR2(50) not null,&#13;
  ROLEID     VARCHAR2(32) not null,&#13;
  MAKEDATE   DATE,&#13;
  MAKEUSER   VARCHAR2(20),&#13;
  MODIFYDATE DATE,&#13;
  MODIFYUSER VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="69lsp702su58klccko1lnmik60" timestamp="1571735918753"><title>角色菜单表</title><position svg:x="289" svg:y="116"/><notes><html><xhtml:p>create table CMS_ROLEMENU</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  ROLEID     VARCHAR2(32) not null,</xhtml:p><xhtml:p>  ROLENAME   VARCHAR2(20),</xhtml:p><xhtml:p>  MENUID     VARCHAR2(200) not null,</xhtml:p><xhtml:p>  MAKEDATE   DATE,</xhtml:p><xhtml:p>  MAKEUSER   VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE DATE,</xhtml:p><xhtml:p>  MODIFYUSER VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CMS_ROLEMENU&#13;
(&#13;
  ROLEID     VARCHAR2(32) not null,&#13;
  ROLENAME   VARCHAR2(20),&#13;
  MENUID     VARCHAR2(200) not null,&#13;
  MAKEDATE   DATE,&#13;
  MAKEUSER   VARCHAR2(20),&#13;
  MODIFYDATE DATE,&#13;
  MODIFYUSER VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="0m67o7tm8a7n3tefj950c8n1oj" timestamp="1571735921984"><title>登录日志表</title><position svg:x="292" svg:y="172"/><notes><html><xhtml:p>create table CMS_LOGINTRACE</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  ID          VARCHAR2(32) not null,</xhtml:p><xhtml:p>  USERCODE    VARCHAR2(32),</xhtml:p><xhtml:p>  OPERATETYPE VARCHAR2(1),</xhtml:p><xhtml:p>  OPERATEDATE DATE,</xhtml:p><xhtml:p>  MAKEDATE    DATE,</xhtml:p><xhtml:p>  MAKEUSER    VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE  DATE,</xhtml:p><xhtml:p>  MODIFYUSER  VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CMS_LOGINTRACE&#13;
(&#13;
  ID          VARCHAR2(32) not null,&#13;
  USERCODE    VARCHAR2(32),&#13;
  OPERATETYPE VARCHAR2(1),&#13;
  OPERATEDATE DATE,&#13;
  MAKEDATE    DATE,&#13;
  MAKEUSER    VARCHAR2(20),&#13;
  MODIFYDATE  DATE,&#13;
  MODIFYUSER  VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="7v0a7b1ptmaqjtakce86hqvfln" timestamp="1571736394713"><title>批处理任务定义表</title><position svg:x="-428" svg:y="290"/><notes><html><xhtml:p>create table CF_JOBDEF</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  JOBCODE      VARCHAR2(6) not null,</xhtml:p><xhtml:p>  JOBNAME      VARCHAR2(80),</xhtml:p><xhtml:p>  JOBDESCRIBE  VARCHAR2(200),</xhtml:p><xhtml:p>  JOBCLASSNAME VARCHAR2(128),</xhtml:p><xhtml:p>  MAKEDATE     DATE,</xhtml:p><xhtml:p>  MAKEUSER     VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE   DATE,</xhtml:p><xhtml:p>  MODIFYUSER   VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CF_JOBDEF&#13;
(&#13;
  JOBCODE      VARCHAR2(6) not null,&#13;
  JOBNAME      VARCHAR2(80),&#13;
  JOBDESCRIBE  VARCHAR2(200),&#13;
  JOBCLASSNAME VARCHAR2(128),&#13;
  MAKEDATE     DATE,&#13;
  MAKEUSER     VARCHAR2(20),&#13;
  MODIFYDATE   DATE,&#13;
  MODIFYUSER   VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="24qb50bl747tmjse5q7k4873rq" timestamp="1571736396785"><title>批处理参数定义表</title><position svg:x="-427" svg:y="366"/><notes><html><xhtml:p>create table CF_JOBPARAMDEF</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  JOBCODE    VARCHAR2(6) not null,</xhtml:p><xhtml:p>  PARAMCODE  VARCHAR2(20) not null,</xhtml:p><xhtml:p>  PARAMNAME  VARCHAR2(20),</xhtml:p><xhtml:p>  MAKEDATE   DATE,</xhtml:p><xhtml:p>  MAKEUSER   VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE DATE,</xhtml:p><xhtml:p>  MODIFYUSER VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CF_JOBPARAMDEF&#13;
(&#13;
  JOBCODE    VARCHAR2(6) not null,&#13;
  PARAMCODE  VARCHAR2(20) not null,&#13;
  PARAMNAME  VARCHAR2(20),&#13;
  MAKEDATE   DATE,&#13;
  MAKEUSER   VARCHAR2(20),&#13;
  MODIFYDATE DATE,&#13;
  MODIFYUSER VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="3tvl56h17spi3urefud52b0e5g" timestamp="1571736398721"><title>批处理计划表</title><position svg:x="-451" svg:y="434"/><notes><html><xhtml:p>create table CF_JOBPLANDEF</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  JOBPLANCODE    VARCHAR2(32) not null,</xhtml:p><xhtml:p>  JOBCODE        VARCHAR2(6),</xhtml:p><xhtml:p>  JOBPLANDESC    VARCHAR2(200),</xhtml:p><xhtml:p>  RUNTYPE        VARCHAR2(5),</xhtml:p><xhtml:p>  CRONEXP        VARCHAR2(200),</xhtml:p><xhtml:p>  CRONEXPDESC    VARCHAR2(80),</xhtml:p><xhtml:p>  REPEATINTERVAL NUMBER(12),</xhtml:p><xhtml:p>  REPEATUNIT     VARCHAR2(2),</xhtml:p><xhtml:p>  STARTDATE      DATE,</xhtml:p><xhtml:p>  ENDDATE        DATE,</xhtml:p><xhtml:p>  USEFLAG        VARCHAR2(2),</xhtml:p><xhtml:p>  TRIGGERSTATE   VARCHAR2(2),</xhtml:p><xhtml:p>  MAKEDATE       DATE,</xhtml:p><xhtml:p>  MAKEUSER       VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE     DATE,</xhtml:p><xhtml:p>  MODIFYUSER     VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CF_JOBPLANDEF&#13;
(&#13;
  JOBPLANCODE    VARCHAR2(32) not null,&#13;
  JOBCODE        VARCHAR2(6),&#13;
  JOBPLANDESC    VARCHAR2(200),&#13;
  RUNTYPE        VARCHAR2(5),&#13;
  CRONEXP        VARCHAR2(200),&#13;
  CRONEXPDESC    VARCHAR2(80),&#13;
  REPEATINTERVAL NUMBER(12),&#13;
  REPEATUNIT     VARCHAR2(2),&#13;
  STARTDATE      DATE,&#13;
  ENDDATE        DATE,&#13;
  USEFLAG        VARCHAR2(2),&#13;
  TRIGGERSTATE   VARCHAR2(2),&#13;
  MAKEDATE       DATE,&#13;
  MAKEUSER       VARCHAR2(20),&#13;
  MODIFYDATE     DATE,&#13;
  MODIFYUSER     VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="05pq8if3jjjokn5n10jbeetmki" timestamp="1571736403305"><title>计划参数关系表</title><position svg:x="-438" svg:y="488"/><notes><html><xhtml:p>create table CF_JOBPLANPARAM</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  JOBCODE     VARCHAR2(6) not null,</xhtml:p><xhtml:p>  JOBPLANCODE VARCHAR2(32) not null,</xhtml:p><xhtml:p>  PARAMCODE   VARCHAR2(20) not null,</xhtml:p><xhtml:p>  PARAMVALUE  VARCHAR2(100),</xhtml:p><xhtml:p>  MAKEDATE    DATE,</xhtml:p><xhtml:p>  MAKEUSER    VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE  DATE,</xhtml:p><xhtml:p>  MODIFYUSER  VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CF_JOBPLANPARAM&#13;
(&#13;
  JOBCODE     VARCHAR2(6) not null,&#13;
  JOBPLANCODE VARCHAR2(32) not null,&#13;
  PARAMCODE   VARCHAR2(20) not null,&#13;
  PARAMVALUE  VARCHAR2(100),&#13;
  MAKEDATE    DATE,&#13;
  MAKEUSER    VARCHAR2(20),&#13;
  MODIFYDATE  DATE,&#13;
  MODIFYUSER  VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="4frmem76sg53mm1gbii2u8qird" timestamp="1571736402489"><title>计划运行日志表</title><position svg:x="-439" svg:y="554"/><notes><html><xhtml:p>create table CF_JOBRUNLOG</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  SERIALNO    VARCHAR2(20) not null,</xhtml:p><xhtml:p>  JOBCODE     VARCHAR2(6),</xhtml:p><xhtml:p>  JOBPLANCODE VARCHAR2(32),</xhtml:p><xhtml:p>  STARTDATE   DATE,</xhtml:p><xhtml:p>  ENDDATE     DATE,</xhtml:p><xhtml:p>  RUNSTATE    VARCHAR2(2),</xhtml:p><xhtml:p>  RUNRESULT   VARCHAR2(200),</xhtml:p><xhtml:p>  MAKEDATE    DATE,</xhtml:p><xhtml:p>  MAKEUSER    VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE  DATE,</xhtml:p><xhtml:p>  MODIFYUSER  VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CF_JOBRUNLOG&#13;
(&#13;
  SERIALNO    VARCHAR2(20) not null,&#13;
  JOBCODE     VARCHAR2(6),&#13;
  JOBPLANCODE VARCHAR2(32),&#13;
  STARTDATE   DATE,&#13;
  ENDDATE     DATE,&#13;
  RUNSTATE    VARCHAR2(2),&#13;
  RUNRESULT   VARCHAR2(200),&#13;
  MAKEDATE    DATE,&#13;
  MAKEUSER    VARCHAR2(20),&#13;
  MODIFYDATE  DATE,&#13;
  MODIFYUSER  VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="4f4bju806umt5qne93tdi484te" timestamp="1571736263022"><title>邮箱信息表</title><position svg:x="-417" svg:y="-3"/><notes><html><xhtml:p>create table CMS_EMAILMAININFO</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  ID         VARCHAR2(32) not null,</xhtml:p><xhtml:p>  EMAIL      VARCHAR2(50),</xhtml:p><xhtml:p>  EPASSWORD  VARCHAR2(20),</xhtml:p><xhtml:p>  EHOST      VARCHAR2(20),</xhtml:p><xhtml:p>  ENICKNAME  VARCHAR2(20),</xhtml:p><xhtml:p>  ESTATUS    VARCHAR2(2),</xhtml:p><xhtml:p>  EROLE      VARCHAR2(2),</xhtml:p><xhtml:p>  MAKEDATE   DATE,</xhtml:p><xhtml:p>  MAKEUSER   VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE DATE,</xhtml:p><xhtml:p>  MODIFYUSER VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CMS_EMAILMAININFO&#13;
(&#13;
  ID         VARCHAR2(32) not null,&#13;
  EMAIL      VARCHAR2(50),&#13;
  EPASSWORD  VARCHAR2(20),&#13;
  EHOST      VARCHAR2(20),&#13;
  ENICKNAME  VARCHAR2(20),&#13;
  ESTATUS    VARCHAR2(2),&#13;
  EROLE      VARCHAR2(2),&#13;
  MAKEDATE   DATE,&#13;
  MAKEUSER   VARCHAR2(20),&#13;
  MODIFYDATE DATE,&#13;
  MODIFYUSER VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="57vsu9shp983f18r94at3vqcjd" timestamp="1571736293104"><title>发送任务定义表</title><position svg:x="-408" svg:y="52"/><notes><html><xhtml:p>create table CMS_EMAILJOBDEF</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  EMAILJOBCODE     VARCHAR2(32) not null,</xhtml:p><xhtml:p>  EMAILJOBNAME     VARCHAR2(80),</xhtml:p><xhtml:p>  EMAILJOBDESCRIBE VARCHAR2(200),</xhtml:p><xhtml:p>  MAKEDATE         DATE,</xhtml:p><xhtml:p>  MAKEUSER         VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE       DATE,</xhtml:p><xhtml:p>  MODIFYUSER       VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CMS_EMAILJOBDEF&#13;
(&#13;
  EMAILJOBCODE     VARCHAR2(32) not null,&#13;
  EMAILJOBNAME     VARCHAR2(80),&#13;
  EMAILJOBDESCRIBE VARCHAR2(200),&#13;
  MAKEDATE         DATE,&#13;
  MAKEUSER         VARCHAR2(20),&#13;
  MODIFYDATE       DATE,&#13;
  MODIFYUSER       VARCHAR2(20)&#13;
)</plain></notes></topic><topic id="59msg8vpm8phvpfai5ls0crf7q" timestamp="1571736333157"><title>发送任务邮箱关系表</title><position svg:x="-410" svg:y="114"/><notes><html><xhtml:p>create table CMS_EMAILJOBADDRESS</xhtml:p><xhtml:p>(</xhtml:p><xhtml:p>  EMAILJOBCODE VARCHAR2(32) not null,</xhtml:p><xhtml:p>  EMAILID      VARCHAR2(80),</xhtml:p><xhtml:p>  EROLE        VARCHAR2(5),</xhtml:p><xhtml:p>  MAKEDATE     DATE,</xhtml:p><xhtml:p>  MAKEUSER     VARCHAR2(20),</xhtml:p><xhtml:p>  MODIFYDATE   DATE,</xhtml:p><xhtml:p>  MODIFYUSER   VARCHAR2(20)</xhtml:p><xhtml:p>)</xhtml:p></html><plain>create table CMS_EMAILJOBADDRESS&#13;
(&#13;
  EMAILJOBCODE VARCHAR2(32) not null,&#13;
  EMAILID      VARCHAR2(80),&#13;
  EROLE        VARCHAR2(5),&#13;
  MAKEDATE     DATE,&#13;
  MAKEUSER     VARCHAR2(20),&#13;
  MODIFYDATE   DATE,&#13;
  MODIFYUSER   VARCHAR2(20)&#13;
)</plain></notes></topic></topics></children><marker-refs><marker-ref marker-id="smiley-boring"/></marker-refs></topic><title>画布 1</title><relationships><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="6q46gc9rln8fbpqabh5dptdi42" id="6j4u1pmsb9uo2897gb5pd62fjr" timestamp="1571735389949"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="3mtoo3u6oe0vv0k4mdisd3rti3" id="5lemqinckf726jg3os7bkgkin1" timestamp="1571735551450"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="4sfvbl7h4udhi08cfu8rfsfafc" id="0o5t7rr00raoh9lthllrosh9qi" timestamp="1571735693147"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="3oufor08h7f8j8seifpv1egpj9" id="2uptojutqb7l3ddr2gpo936vhp" timestamp="1571735763609"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="4f4bju806umt5qne93tdi484te" id="4eg7u7llsb050btgvd5m6i03fp" timestamp="1571736341449"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="57vsu9shp983f18r94at3vqcjd" id="75n50ugjf31ujkh4d62th72q6s" timestamp="1571736347321"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="59msg8vpm8phvpfai5ls0crf7q" id="61ccca5lgrctsrvht8hk9j2jnk" timestamp="1571736362161"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="7v0a7b1ptmaqjtakce86hqvfln" id="6he84jgb7caqflhgge5bv2scjf" timestamp="1571736370889"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="24qb50bl747tmjse5q7k4873rq" id="57qbo3cpd8d1ct04vp0o4537no" timestamp="1571736376209"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="3tvl56h17spi3urefud52b0e5g" id="34hvqiv410hpbavvq4ui3mtgfc" timestamp="1571736382185"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="05pq8if3jjjokn5n10jbeetmki" id="38vs6intq1m45rrfdrdk8dtck3" timestamp="1571736386801"/><relationship end1="6hhv3lsc3pn06bh78adhm0v5qa" end2="4frmem76sg53mm1gbii2u8qird" id="2kqdj9san7ulh0a2no39rsb425" timestamp="1571736391722"/></relationships></sheet></xmap-revision-content>PK�&�7C  C  PK  ��VO               Thumbnails/thumbnail.png  ���PNG

   IHDR  �  �   ��?  �IDATx��}xTչ��?��x=�<G��<?�ﴢ��GĖ�m)�*m�jKDA���TĀh		/	B�I �H !�W�J��!L^���Hƞ<�F��7Y�������u�L�s}��־׺�u����|g�=k�����G!�B���3 �B!�ݠJ&�B!D	U2!�B!J��	!�BQB�L!�B��dB!�B�P%B!���*�B!�%TɄB!�(�J&�B!D	U2!�B!J��	!�BQB�L!�B��dB!�B�P%B!���*�B!����{2g�<|����L	�V0:�q�s�����s��*�B!^΍����?Z��c\������_��
F�1b�?�|vEL��]���P%B!ěɻ�}n0���>�H̶<�ZXR�Y����P%B!�k����X|Ŧ�`Ջ���;/����XxTɄB�Z�vL���L��������XxTɄB�NR���jit{���[<�P���,��	!��,K_�{�K;�e(��>I�#�YP%B!�;����G��/n�I���/ܭ��,��	!���5}SMK������L	���xTɄB�N�oܲ� ��ց9^��12��~�?�g@!�2@^�;�\Ykp|���z�ؘx�@#� �f�'^���gK�6>�n�  Ur���3 �B�U2D�c"���u��vd�-h����O
�;v~�+-�*�-���A��L�Xm������=B!��� ������'ߍ�[ X�'��4@3��A�K��]��s��+�PZ.�SͰG��@L��u m�u�+'5��M�@�C/��~�?�g@!�2@�޴;�T�h�eE�14�$���9tG���u�=��|�7W�w�G �\�����Ԏ�B�F�zQ%����=B!��� ������*Yn�`I4�-h�f�Q�h,g�ˡ�R�BH����ñ�ܡ�6Hy�k�ng�֡Ur���3 �B����;#1����p���%�ЩrK��ͮw��!GM΂;s47v�^��-6E/I:İ�_�D;��;jzQ%����=B!��� ���fw�Ѭz(]���]�mGMr��CwT)�3'46ݢѻ�#P�rO��WR��_�%8�����}��!�B�p���w*��{.<��\5wNߤ�M��)
�����U��E ���UN���1_�R_K����*yh��3 �B��7��ؖ`��,VnY��`�[ ����'.��9kq|�������_ߐR��-,�;����.m����~ӑ��:��J����{�B!�t�vg|�� Z�X
�Un�wN�c�C��gm1�l�`�ζ4w��"X*���Nh���ھqk��͗��K�ؔ@�C/��~�?�g@!�2@6^�;��eaF��[���_�������c�z���@"C#�؜�,6����'��E���Ǭ��o�*Wp"䡣��m��5�;��J����{�B!�taC���>�?�k�[�J�[���3�վbJfj�+����E��,�ƣoFT[�]���o�,
�������g^T��>tπB!d8�.�o�;��ya
����GLr����z�/Dmt�E#��+�n_Sr��D�׮�*@��+����ZyϷ�*�>޶�^/��~�?�g@!�2@ֵ�r,�:�D�q����x��-{�\��YD�vg�Rd��~��bm��D/R���V�� ��gmA�>�E~t���K���E����G�!�B�����C��i,��T_�J>lB�l��PF=�wNhb�Uަ��{�;�j�~` A ��~��d�厩롕aGy0]��J����{�B!�taM�]MAUg�
�}AP����t6A����M(��|��\��0��@�#7Had��i@��5T��>tπB!d8�.�4�՜<��Ю�h����N�c��W|�AX�����T��>tπB!d8�c�����MvB�< ��	!��L\��e�]���������xTɄB�NmN�doA��N���<c�!ݏ�gA�L!��dWR�kW�v�����Y�ς*�B!^����gZ��죙��������m��gA�L!����qoD�j������o�]q0)۬���8��	!����6�L\�7��v��>�(����rO��G��J&�B���YZ�؂��Sc��
��*��M���Ϭ{o�ه_�ɫ��*�B!ޏ�/�����s����)^�]�7=�4j��,ދ<��	!����74g=�CI"Ϙ���'tϊ�3TɄB\xu�����~V<���KM��D��dB!�x97�ḱ���+Y?�*���G��=+��P%B!ě����� �o����i��_=Y4m*ʺ'F��dB!�x!�Zm�A�1q-Ɯ��fa�8Ο<	��#�U2!�B�������}}oV�*�x��U2!�B�(����g�FA��	�TɄB�x �AѴ��2 ��	!���@ׄG�M�И�Ȼ)�B�L!�O�fu-$r����<2�P%B!�����M���{&�[�J&�B�'}|����׏ɰB�L!�� ��h�T�?�&# U2!�B����(<[ɺ'CF	TɄBq_��Kg�X4m*�1a��	!�⎴s��
�ܔ��{2dB�L!�����/oℚ�.�L�*�B!�����r__s` 
��D_��	!��?�Zm������,!۩��;@�L!�=׏�&N�8�>&�U2!�B����Y�?HuP�V���"�*�B!#�q����	�	��'C�C��	!�2r@7��]/5A%��1qg��	!�2B@g�}���W�L��dB!�/�o~Yq�Ԅ�յ��C�+P%B!d���&N0-\`���=B\�*�B!�BMx�%���&ݓQ�_޴rO挕����)�
F�1��s.��^�}�qP%B!d�)x�i��n��o�w�_o�����2�u��j�V0:�#��O�+bj�����*�B!CFCL\��IM���ͺ'�&�R3�q��t�+�h#1���kaI�fݏ��@�L!��! ��:(�h�T�!Y�dr��2���Mw���ױv^��������	!�2(�R�!�/�����K�4�2�::������O-ݯ�����	!�2@�����g�p���)�k�4���N�?a(����?TɄB�7-Ɯ��/�O����Y��:*��v��P6}��G���J&�BH?�^jj�/��lo���=�����G��/n�I���/ܭ�q��	!��7�kM�M�Д��{2���jZ�l��|gJ��G���J&�BH@���k�#��'z΀.�q��
��V[*�<�b`��W;��/��]:gtπB!�L����q�A���Ѕ�;�}r�Ȋ��3-�4��f�cp|�d���կ��3<�Q|�T�.�3�g@!�7�����.2�-��V�M�|��*R��ő�s�о�������B�{fm�6
�ۑq��M��Z]W��Qn���}��^g��jC�<�sF�!��n�s��c/���¶v�6�
�P���Y�r�s�Ƽ
��#��c"��]�����|7��lO4�+�d��/ m�u
Ц�J�Fשau�mrjzQ%�t��!�B�q�8��7���%�\����]�����˩�[�XY}�K۱��G<K�C��k�^jV���r���O�S;�n��aw�E���9�{�Bѝ[�6(c��r_ߛյ��3�@�ܴk ]{Ϭ-�9�����t�D��2,��xVx�;Ƽ�Sn�,�m�p�6�\`u���B�\�������Ny�k�ng�֡U�K��B!DG ����sƏ��=��y�@6aw���F�6�'*��A@tA�h�-P�n�{��&.���]�%MD ��DC�*6v
w�U䠑�C[�uK��kɰ�֡U�K��B!D�����j�#L��{>�
ta����ww*P@���a<�U?fN����T5t-ٞ�g�`�Ѷ59�� -��ߕ{r5������-��u�E���9�{�Byb��&N���{&#�3�\���+iG�e�c]p��-�,P�dQ�J���Sf)xl���� ��G ��ԗ���|mKq|-ٖ�Z�䁟3�g@!����X�J��ˁ.�ްkӣ�/w�r����9��j���d�}9dq�I��Y\�v�5��S���	0 ���h�!���.m����~ӑ��:��G���J&�BFM����'��~�VQ�{2#t�vm����Q>ҫ���ʁ�}ks԰ J��)�&j�ѩ�W"���2�� t���08:�QN���}�e��26%P�l����*�B�~��������c����ta�u�6h�Vpڲ0#�ؽs�&Q�6��C���w���XyVJ�;յW�z$��"Q�Gߌ@{���2[�	��5���W�
N�<t4���?ܷ�~g#����?TɄB�7���\4m*�P�=�.lh�k�W��*m�g�\K�7@�Q;B%;�+�S���e��t��ɸ'ٌ�}F�����7]��y��x�3/�d���3 �B�p�b�)��*TrSj����ta}�]��Q�Ӥ�ý*Y� r+:Ԏ��
 ���k���
�x���7�(�H1Q�gL��o�fU }�m��^T�.�3�g@!��!���/򤆘8�3q��Z��0_�{֖��V�r�\�J��A����/m��Fpp����E��e�~�B�����,��r��U3?ID���,�aA�Gw�ٸ�{�^T�.�3�g@!����z�ɴpAuP�W��`�.�m�;�È\ ���Q��fUc7"d_�P�N� ���F4Ј￯ ���M�*�m3V&��i�Xy��1u=�;�CUk T�.�3�g@!���Yܖ_���΀.�i�;dվ�\�1.���ya(6Mz'�;�ɡ;ZBࢍ6D�:t�Fn/}j(��RTTu.J[w��Y��*٥sF�!�2�����n��tO�m�.�4��Ͷ�fԫ�,]@�|50%$��a�A�u�B|8"k@���9�{�B��7�k�}}���)���c�����MvB��"TɄB��!�</o�ƄDݓqC�g��y��/�n�=,,E&dYuW��@nE�}sCt?F�U2!��I@7��]/5A%���3*?��x��%�'�|ۼe��-���ɾS�g�<��1r��	!���8g�8<랉�c�0�WH����˧���������8�v������J&�Bܝ[����륦�����f��qg��-!�Kg�������c���+��E����gZ��죙��������mݏ��C�L!��5M��9��]����ΰUT�EF�.�׉�������~75�ᇪ�7�.\i�F������>:�n�����ͺ2��*�BqSj�# ������tO�݀ nLH���D�F���k�v��<I�Ȃ݆������.7�G%շ!�W�����y
TɄB�;R��Ӧ���4��W���s �濊/�nA�b6�홥u�-ؽ085&��������ݔ^���̺�v�}������/��	!�7�!&.�$�@�,a���nLH�
.�6�w�7�����).贈QwM���)�ƈ��ݟ�{��U2!��@C��~Y�dt���/��d �6���6���UP%B!:-X4m�%�3ѝ��B�t��L��{Jd�B�L!��Da{Cs��ʺ'�7�k��rƏ÷��`�S"��*�BхcN���'O���*�Y,n�@�%H�
�dB!dD�^j�|1
o'��!�/���*���@��*�B!�!�'OU?DèŢl�
|I�UT�!}B�L!�;��徾Ћ���1dq{C3[���y'X�Pƣ���P%B!�K���bMx��_�̰��m���3g��>Ƌ��W�P%B!�$c����^��o��lU�||rƏ�����w@�L!�=M���c�
��u���?yR��QK��!CU2!�2d@/V��<���_z�m��90�h�Ԝ��P�	�����C�L!������P�^��-!���j����Zmu�Qm����D�@�L!�
h�������~�Ƅ�K>>y'`PP�M��^|k5!�J&�B�q[~aCL�X�M�|	�R��_4m*Fe�`P��dB!��H׏+��tOf0@[B�Ϝ��@�yC!�dB!�@M�_�y�b���>�}}1�c�yC!j��	!�W��k�y��H�X,i|��B�7T�U2!��7Д���m����=��hbb���`�PA��P%B!Z�74M�
��)�X��G���V[���~~��=+B<�dB!�1VC2T&D��_�}�˦�ts`��f,n��Ƅ�dB!D	�%�fѴ�ʺ'���R��<��������hB�
�dB!�?i1��~����m�?O�Pі_�$����=񧄄�?TɄ��v��͸и|W���?'�;S�(�_.;��#�=1O�L��	��_����K���Y�3~�%���t�_)�x7TɄ�_h��լ5������gC�L-�ֿ�8�p�T����_/?Xcm��B��*�B�����{#|]\��k%ĭؕR����I�f�_&����	!�?������H*��5��7$�������ko��b!d4@�L!=����/�N�4����+Bܖ=g̿z7J��!��dB�!>��	�}��_��p,�P��K���*�BzX��Nع���qs6.��>I��!^U2!�������(/��$�͉ͪ���ݺ�d�z��	!������gʿȯ�$���Δ �_2�x=ޠ��˛V�ɜ���}sCu_�k���.]��\fi�� �}��KB<�dBF �V�7ڻ�7�ha��{�q抺����!;�;�g>�Ϯ��R����ȹ�%!U2!#���K����ӭ��dXI̶<�Z��'�dGV���xT�C�(�������T�|������Mw9Jh��Υ�7�ϒ�+�	���ɨ�������T�</а�`�贓#�|�SK��~�	& ;Ιo�P%��<���~�*9�|���F�w��3o�q.eO�Ȏ��ۄxT��sќv�T����WG����NF�]�2.eO�Ȏ3������99�:���~����v2�d]l�R��[��H��E�G@�<08���~�*���jZ�l��d��[3�Vpn�.� �#�[���\4'���G�d�;ܸeנ��S��3R��jㅫ}:Z���<�����yr���Xw�o��[���r�c�14;W���u����S� l���Q�#��9��=&�Y�l<V���v)l���V<08���~�*�z�]�v_Yg�n�&:�|����s��ƼJ�;�i��<X�؂i�����w�ϕ���;�y9�t�U�\������c���î6u�w��o��[��}�b��Tx�p��̙3���W�\ihhh�}��MQ���m���!�;��U��fdf�T����>5p��C�����Ҙ�SW���4;k��퓘��&�������C��6���-�#���V<08���~�*�Q�#!����_Zݡ��̅�(CqBgC�.ޚ6�?Q��olL�V�M�,��ڗ{Ϭ-}���vd ��#
�R>}�dŷ�̵u����P%�Q�m��}��O7�H>m2��2�����}� 3�� ��x�1^
Ly��<Q^�;0$�����������|��HTI-�-���-g%�+S��W,�o�p�#"��0��눴�y�7Z��x�/s'N3M���Rvֲ���uwN�������j��:E�G%'�D��J���]gHʩA�{�#NV�}����J��]�+[�@������~���Yėzybq����su�s{����y9ԡ��J��02���Z�A�adAj�C�u���Z�^|Qo�vRY��{� 99����j����ի�F��e�z1b�[����SQޚ\��р�GJ�����F�f(OZ�zX8J����9k�Z�q����l:^����>dR�q��?���o��2D�Q�MC���V<�����҄�+���Ȑ�4�@�ڗ+oy�w����^_sv�����n����֛v5O.�^�%mE�����Q��� ��*��h����?mL�;V_����X<��R`�	*�p�(mE�Rm����6����u
ں��˩w"�}х��d/�U
BM�#� �>�N�x��!�j�ݡ_T�[��}�B���;s�`0@C�^q�fh8I#�ץ`��H�ݝހ��l�y��I4ؘT���r�c
��P����zT���}�"���"<�F�ڨ`ƚ�h�
U���"����1�Ha�E΢��e��P��uiu�|�Y$�\(�qt��u���a��SUr�M���Ĝ��^M�hB���-Wɢ���N�#dn����
�ۺ!���DEzi����"���s��+׺�$��Q����HOᨁ]�_	��������T�������@�C/�����s�h��Ar8�>!�XUUUuu�e�h8�}�9�$��j�����9-�g����s�bˤs6�����Ԏpqs��<
e��,�vR��#�<�����v�H{��<ߊ�2w8MZr��wUd�4%�33���o��.ݑ!���׻�fg\h���u
��3K�؜vg<U%7aW3*9�������P���k�P07v��Y��m
�:D���[E9�D���SjGTI���s7^ow  � !�Dl��\j� ��Ԍy9TGM]k7����Dp1�~a����[�^K����/�kI'*W�hoh��� d���>R|s��=�r��y��R��\����0�De��9�L���3�=t��Ӱ��S�(��Kx�u��dٖR���r���=o��{
f�
\Q@{<;�ѷ�j;Dm�ْ����@d;T��r���;��.Z�o�2we��1u�T^nL)�f��.ڒ�lVy�Z�,�D�r�ژ"���&>�ں99�Yx�Jn���@%ͪG��]�mGM(`�� �� `?S�����еYmh9���(@�)�b����aw��RP��,�6Ha�H�9}�N� U1LEnooN��J
���g���.�!h+(>��/��}?�G��st?%<=��}1k�$$\�|��ŋ�������m(�b�}8���$E�A�1̿>�����]��k���7`���q�oxi�i�uG+a|��D���G`�3�ښ!ܑVˊ��Շ/! �,�S�2@T����bS���RѠw��
_��E�pA��F�N5��<���t�At�0���?/l_V����̵gY%�\�J/m�J5C��zy,D3>�ō��f��)k�)�F����ǨS��
E�MQ�d{"� )��g)j�)��êD��1sB�U��S�JVĔ@X�J�<e�C���őb�rz�j�2j|%8�q�׶�גm)�u��/O}taޫ�ǂ��M�J&�A��_�=ǲϞ=�k6�V�^����a��a\�w��emB�gIW�L&:���K��u�*��j��ٕ�Ͼ~�{];p�3��-���-���K�w?/@3�ޕ�6��_\�{s���<���d�8���1�{U��k���ȍ���;x�YLt��
�zĽÀ��`��q��%Y��J�z��\c�56�"&�C��6*�愥�۳���|3�ؔ�!kL���a<�;9L�*�zîJqN�ay�E��}�6�P(�4w��r}�����y�m	&�+!@�Ɯ��p/T��ʮv�_��Ds���0�X���Y[���K��R&.�|{sz�c)i���o:2��Z�^{�N0�?FR��9��wϖ�~���)5���RSuP0��������lUCU��$'#^���_��c������ʠw���W�Z����aw!˫W�X}������|q�JQ\�<���Żr����x K@B�(���U�.��c�o?NrV ��?ﺢ#X^ےq��`y_�n�+C�R�����o�ʄ*E
��Rc��f�؍�{UrHj�dy�߀�� s�����C4���H )!ڏ�GA��~}��F�Q��Wh��U��=z-�D��lʵ-��E���#��U&K�S��2T�23<�͈���M��S��O#��?K��a�����k7�jp�1�_땳[L(`����hv���ijw�ӈ�f�ŭ�DX�J� ���NQ�J>��aJ}"T2��� @�"�z���B2�f�b���ªD�ɦ���{�|Y(�ƉM	�:���ˊ�?�7q�x�)���kvG��>�C%����[���,��m����p��o C��r��6"�,�}�?�����ŋ��?P��|�C�B����ƍmmmuuu����bԑ�Z/��?>�
�W�$�*���Yj))]��5J��*Sۿ[u\��/|�D���ǭ�	�.,�N�)p���D��If�����H���K��Q�L�ލ��r��މ8��i(v�ܲ/��9����S�#��l#r@��y��i;�E�-�9C���qI%���/��4>´E��|�9�Ym�1���Y,�Щ+��:sT�cS�ikh_19�-�FwS��*&���pL�,�OUɍ��j~�N�JFaY�q�
B%�2�l�:XQ�%�M-j�;"�Wv�=k˞3"_	y9Щ��>υ�\� a�\Z�	D��)�jS�Öj�̝�7I]��I"���g,��Ǭ��o�*Wp"䡣��m��5�;�/*觼'���O=�w\�����!W��r[~ᐫd0z�����������#����4���x����***�ꫯ����sW�"��;{��ݜ�ir;6!���G�~��G���3�SuP��V~#���$�~ի�V���c/��R�i�hr���!�x��(��!�؜��A��!��n�]}�х��(f��@�c�@ࢎ�ZT�-�V��8������>�/����<	���a��O���+�{{0��S��� ,��z��	��ks`�A8J�( �x��^V����'�����ۛ�>�+�]�+�eQH0ֿ�!E�KL#�7�s���igA ���(��0Ur�x�Jnh���̍ϬGA�d�9�S�� �%"�Ut�}�Y��| Ͳ&� ���"�T�.�k90�I6����Vm�.��@�Ζ �se6�#Z"&Ƌ�%#r@��+�w��h��~�eQ }������8�^T�o~����~�7b�O	2��o ��rYTލ� �{���l'�✜���333����j��X�����<���=׀�~r\�cHZ�T~dA�J�úS�6��� aV��B=�Ř$����b��H�����f�,�W�hQ�b3�h�[;rDv�"Oz/N;�H-D�/ߏG��	�+� ��0t�<s�fS����~��z��,�zwo��
Y'�2�����m��F@%�_S~=�Q�Ea���Zr��q�?^Y���H��?���9���.�|/
��/Ks��ÎW�g�ń�`����O��S���6������o�a��0MS%������6���Ù�(��71�p�W%�_B2�	v$U��pl��>υ��WJFDx��8J >���B��Vt�2�]ˁQ$&�Rm�9
�iDF�EKDJ�W:\�&���Q�BK�ʫ>O6ÒQfs�D���ۿY@o[~����E�e��׀s{_�������t�8w���իWKKKO�:UVV����*T�[�Bw��\u��?�vHm����zU��9
;,=�O�ڪv�Q��w�$�[U��ן���@�?���qg�U���ҸO�P�0�(�W�ҝ�}wO�t3���jy��Q����1^W
Z"�������D��^X{J�alQ�zj����F_��Aɵ���0ȳK��+@%g?����s��*d����Ԣ�ea����GH[|���&��<^��}�����E�f mŜ�4o\Q��<�|r��Y[���>I4�Y��pO<U%׵��@kB���4�y��Q��A<�PۏU<�F�M{�����Xaey����k���"��_��r�;D.pT4��йz�qaP��OQ@2W�"``L	
�Qx嘯u��g/2w�6pD�R��d�h��7�WJ��ݭf��i{�EE���{sn�ͻcRRR�ub���ٳ� �5�����ͮz\�~}KD�<�k[�H�����g�B%/؞����,���U�
�.��w���W���W��t�v�����|xTl�9R/��]y����F$���_ܐ�¦���
l&U��?٫�]9(?[�+�F�+�Mt-���z7:c��S�c�s��Ey�Y+�Ż����­V[���R��/s�[�oH�g��ޓlv6O[^��Y��e�	�P}3.��/�����[��h9|������k[�j&�}(�^n��Ӿ�(���P(��8i��9[j������M/}j����(�T;�!�p��A�h)i�?�"wA�Kd�\Њ����86�tU5vc\ǋ6pD�+�ZJ��/��5�aD�C���Vpn�}}0�?�������&{`*����}��ݼyS�����ŋ����|n�I$��{��m���l����.B�*\��\���:P0����ǮHm>;Qz�����D�(����l�Gq�R�;g� i�f�Gc��Aع�0�D��a��BA� ZJ�.��+q�[xm7K�/oJ�"K�9숋T���"%d�݋}�� �+��x�/sW�Z}Ìb"Z����<-��j9�bY�4�,f��>�-�҉ Ҭ�����=9L�0�g0���Դ��D�Z�j��ˍݢ ԪC/9��A�MP�q�P��@�f]�e�����ڈ����&���3	��Ai��"��7�E�R����Ei|Qo����a{r��m����!�O��{��G���޿�_|���_����{CO^�ǜ�)]\���w���������*Y�"T�����<k}�������zC�����+��R�*)�؄�<ڽ���D���6���Xg�/�6��h������I�����&�E4Q��aX��>��o�Rp�_ݒ)��H[;�����������e�=_*捥�di~�bm��"��
��n���m���x����Y��619��{��7I�ݜ���=��$=%��l��N[�_����F�|4�
/y���,]j�7��$�����+]�ʆ�U��Y�����s{��� Y�ut�ٳgO�͟���C��>x� 6�fsWW��|���_}�UJJ�'��+.�["jhz�v�c{U��!�
;,B%�]�V�(X��$VY��R]�돓е|�T���?M}-�]��>	�;^#6�;{��"[�Q��=nI���B=�xĔk�7uXX�%@_O��|};J}� s(���/�tҀo�~�kL��-��X�|�$Y^�� Mɚj��A�6��%.��>Ox�d�;�'�S?��O�O��G�o,�prx�O�3 =��w_m���*�x18��2�ɶ��n8~��ɓ'�����> ������&Faǎ�=u�Taa��d:�<���5pW��d�P�/m<��.�l�T*��mي6���v�U�"(�-����P�U��t㊃�z~�����j�~�+a��C���$�pD@��P���B�;wV�� ���
�,�a����[^ 2AX<;<m��~|�r�g�3�V<����i�ˍ���8�
V�!'f[�(�U1wݧ�6���a�:U����pN�	�{`�Ȅ,��q�[�~���O B�����sm�'0�L``��`��=��H�}�����>P���������ģG��]�vݾ4���:�ܠ��?pIn��^�-m�}�G%�ߖ�p��+:�e�Vu��U�r�I����u�fA�E�?;���L���S>J���P��;�`����Fg�ݿ�)�s���YP��$��l�_��n��щ�_�8*�\U�m��0dW�,�9�(�����A���u�CrR�������4�����Ϊ�����K'���Tɋ6�~����j'#̾S�g�<��	@�p�����!a�Σо����P�������@�0�
���pqmsj�w_
W7zcϳ��xnu�����C�*y��,�;,=*�[ՑaT�����B�JA��fߟ�scr��$�Q|�`4�џ{��	�u�ka�����P轃9W{�$^Et-u�2�Q������>Y}Q�;����<���1�������_���VX���ㆳb�aD�n`P��EKP%��G��]I�/�1\��������Y�� ����v�u�X���麽{�?~�ĉG{��(È*4@34֎|�鷟�P����g�(�*��-Y
_X�JV��W� �����o9?{��ڤZg�=�~�=/������� i8k��'{$�G� ;�E�O��?zUgEL%@��w\Ԣ�ٛ�ɳ����W٫C����~C��eqP�N�~{�}�q���Ͻ
��_<04��7�s��v�T����{�3��kv2b�V�~���M�o�~�	 ;��iB>;ziE�իW�رc��������	#�� �\�	Q���;ދ�8����������gQX�p�a�������񬮅/t-��F��r�����֟h���?X�����X��O{������}�i��
`tx���آ��}�*y`;J|��������p\����?��������B�<08���~�*��qoD�j���d�n�����ͺzB�	Ȏ�i-CN`|�ʝ�>���G���	�������(��?==�?y��
��л�]s�F]�1����Ġ��qU�Z���n�����h)���؊�j���T�"�2�u����>���o�9�4x;�hU���\4'�����d��P2q�ޔB��F;VJ�oC"�ܓ��A'd���Jm!�`hpV�pWќ`�d�vg���.�|l� �J����K?��V�k\��v���l1X]U��\4'�]ǃU2�,�{l����1�uU]�v2��^���̺�v��k�W���ٱ�t!U��\4'�]ǳU2���uS\�SK�I��2�K�c�����M�ݴ��s�����	����h����p��x�L!."�pSj��RS��A��oCL\��(�槯�4�P%��6���A�L�6�j�l��P��||���iSQ�,��hs�旒dǺ�&B<���3��99<0��	!�
�.�.����Z����P�5��CC4�$'����	��	!�\�.7K�(�p]d�E�[���ٱ�D!U2!# U2!�-�}�Kq���,�0tp{C�(WC7&$��C� d�j����*���*�2��հP��3g�,�0좍�wJ���[	���	��	!��.�
��
8{��K׆�6���٫�W&Y	���	��	!��-��)5]�^�+:�}߿�jes``g��k����\�P�ѱk��9�֟��m��mU��v�V��	!���Oeq�%��ɓ��oVע�m�\;��w��Y���k��9k-gXB�����EF����U���t�>!��dB���&|�
Ջ��g������ϴp�����"֬ ÔU�W$4����/�����>�	�����֢iS�V,��+�υ*����/>S�zoV�V��g�} ���XE;� �S6)z�/qˏ4��,�|z��,��Y\T�n�?A1��W� WK$d�A�L���+>#�ź�9����jHV�a~|>�f������	q[v�5>������^�x�C4�*�Ģ���W=!P%�=��O�aq�X�ᆘ8X*���mx�3.\i��ܝKbk�;�@����7�&e�s����N�u!�� ������a�*��JW�7,.�M� &U����IXR��oD����B܊дH�{2����V�/K?B���7�Qr�!ΠJ&�}�Y]+�0>�b��&��<v��Z2K�y#|�'���]����K�ё������>��k;y�u��_���*;Go;��6	a��	�[E�.$����	��Wt����f	q��@�lG�KMWv�Jz~�SK��;S<�瞘��>�ɛ^��/L�+U�~|�(�槯�>"�I�Sq����ދ<������h@4�?�ĳ�/XB��dBFq�W�)5ܔ���qmX��F�)�6��y������8L����Yx,e�_-x�i���V�?y��{N���;���ٻBB��q���'8��N%^)y'\������y-�eP%2Ĉ���3��6�O��E�a��ݖ_hZ� �ۋ�������Wp�����\���'튢iS1|8B"s�]�:�����h�"^ U2!bB�BN,Q��/�C^@���_h�����w{���A�xy�0���;s ��gΐv4��
�3�1�A2ĝ5�8��ьN*.�A<�P���M+�d�Xy������"F� ���=�2K�u?�\A�a1�QA�7z��g�} ������q��4>�q���^��-�B���%d1p�w�8]�&N��"c�`Shk�g��xx���� ��Ή塚�b���i��qw�|��k�zÏF|���a����W;�\pqq4��슘k��� �A\��
�@<�t����O�ۺ�I+����x�?�e�Srpr�t�;D\��t��ǰH�P��k�Nx
2���T���&�Wŭ�u2qC�Z%�]j�>7�n}e'�Gb�����Fla#�\W����e�aHa����\ �pq���>P4mjMx��)+�g�Z�H 6!���k_q�<�
ap։��ěp��	P���@��!:�*�F{$T���b���q�w^��!?���q����ߎ��W��&�p��W�Z��/��
P{���!������B�Ću�8�-!۵/����=�jH���^\x�`_��.P�?�_��H̕���t�w]�C��<?���*y^�a����i'�M������%t���{]_�J���
5,~�/.H;�^���h�>�8��.��(�j���Ր��9xEH��ɂZ!�d4\t'��Xt��/x�il�.�.o"#�����Z��i'��y�GJ��W��Kb	�G�Mq!P��*���(�p{Cs��IB�v��uz7�y8ܕ~~8O�g�m�"�BƐ�'��*�Ґ���"^,�k
��*�"���>4B\A,�!��${���b���\���.-yG�!�MU���Q�7�����.C�{�w��x�����/'��>(nP+�6U�a�C~�����X�Z�P���8
O �3D�Kȝ�,�o�$/�4i�e�_�.3���/�qs�gx�E��4��f�Z���s�Ϟ�z��җ��w20�T%����#F���d4�u���	�7���R�r��S»�.%�C�)5ߑpn4&$����r��C�[3�V�~��ٻl���!Y�Kŭ�����Q�W��!~�
�����4^�b)�J3����B�`�S�O�9�5ᚳn������v�NF	�L^R�lY��<�T�C?,�9�wI�N�զ���-!�Ś$�g�/��(.!��/��E��;=ɂ]*ݚ|��طҒp�x��@��: ]�y"}?䚳^��9�*_nܲ�Bj��z���ƃ���UY�9`��Lˀ}1Ɓu}�j�`�<Hw�������Y���_�<��Þx=���@��n���Y�v��q�_ �ec�E-�%����JF�{�I�����g?26�g;�欷3�5g�W%_�;�\Y�զ.Q�埸xk�(��x��ڍn�^y�6 �����1������wM�t���V�D��1����]`�H��������,���_ gg�Z�J&�
H:���ey���#.!K���v���z��W��{�Z����=2ڨ\�<��	.�1�W^\sv4�p�Y�H���'�O�*U���0v~��C;��Pyc�mX�T�3��L�F�.�+^P�wL]�j_�3��?�G|�r	(�{fm9�[��G��|s��	ЯB�k�W�c�~�p9>V��QNMxD��W��>p���A���B>�mU���|ـ&V�8��Ԕ�.��	Ub� �GJ��p��Q�b�Y�q_���nwH��9{��*6!4�*l��'G�;P��v��[�z�'�P�8Y��S"5�B+؟j�̅XG_�tG6�r�C_������[� ���:��������̕v�"[)��\�'P�H��ڥp)�ҁQ �� B�y�m��^Aj�C�u���Z�^T�ލX�7o����X�X���q	ٕ�>4-\ ���X1Z��!����b̑~�G�h�kΎ*Ě��=I�W%�޴;$4�4~A�(_���S4���Ul� �r�Um�A�J�D��E[�P��ܵ���Vu�p|�/^��;KU���cS
��R��'*�Vѝ3�GdA�C_��ԅT^n�-���݂}�>s(vW�.�v<���g5��#��:2�@�U��<󴸐	��*�;
{����EӦ��R��
�[~9�~"�DO��oG&��kΎ2v��O��I�*��]M}[�C�à!����5EY��M��【D�%��'�^1Azi��=���ҫ��u!��^{�@��UN��3k����a~�7W;�C%H�Ym\��bm��];s�r�K��g�wN߄g���C�ں��u�E���*��u�Q(�WT ڈ��?���X���\�
�,����^M,�pA�1!E���p��QE���/��ߓ�}Ur�v�$��J�{s�A��Tcn�M����	 .����R������4��6�W���%�P�Ӑ(��x?܈��Y����ng��B����rΖ��w�����|���Z2�u�E��@�5�ĉ��������;��K��E����C ����,�)����2�ᚳ��(�U�M6{�<���P�0ֶt����-_0 (TE���)ﮠ�jX�`��S��n;jR�bjd5��D`����p<�U��.�Ƹ�����MHޕ{r5� �V�H1@W��@} ����|��m	�@���t?��@7����\�.�
�z����+���.v{��I�����������B���k���J� ֫����;p�< /�f�[p<����dGx����$�����]W4ܝ�7A�Bʁ��|THaIz
Qu��BnB���*�Ol*�%����c�*��S�]�t�T�S�cSޑ6��r]�
Yq/m��9�Y�^$/W�@$��ˍbשw��q�׶�גm)��J�\���,!��}}Q(�9�7T���f�I�/!CࢽB�j�9�ȗ||���/:��B�h���j_���zgZ�|7��ZrJ�;Ƽ��zVbI+�&_��E�?�m�,.����*�B���o�W)������3k2ybq�+	���
cC�W�d��61g-�ߌ(�ڹ-�$k��a�,�ġK��~N�Aa�t��>�w�KZq��]F����&\
,	̀��SfT�Y�r}���h��:^q�PX`/�܁~ſ)N\�2�+|M2�h�>w�ztbo`GA�ȷ���{��-2"H��7����C����MG�3P�Ћ*�m��7TAV��'��'�)5��:(�ŋ�⯧M���+
⨵/�|�$��wC[%C,�4���b�V	Ԏ��
�~̄�_����i�-���q��>�� ��K��XpV{�V�cA{���Ɣ�,��%���X�]��l�s�����לu_�|�]�ν���z� �0��ªDg.GzU���	�*B��Ĕ�ۚ`R�¢(�Z���\ O}I*����r@n�U�f"y4���_� }�% 	�LЯ�km�ם�7!7��5��܍�<8?�َ��[��o�,�_BƦjzQ%��_U�����K>>u�Q���K�%dW�z����"7B"�M���i��/|!������Fc�Y �'_ݵ�J�%ayԢ���_����fk�
�*lKwd8�W,wi֥�bW��z�۞��d˼B�B7�3��T�;D�!��ᨱR����P�A�K��!=��=e�Y�Uɍ���Vw>�(R��6uC��F�8<;�*Ynٓb~�D6Ė ��3g�p�rĤ0¢(�0��&�Xf��NiiC#sg���h4����<�/��0�Y�Wc��I-jEci�����wB3>�<���5���W�
N�<t4���?ܷ�~�^T��X��fum���gΨ
��D-B�]���b́V��w �D��Sbl*�� �4֜O.���'[l�Q���E�����u��+T/B9\Y����?���Lл������2J[�<V�u�"�RAZ1V����]k@_�ab�YO_s�}UrC�]�i��I6K��tP�Д�,^���?5H��[![�����S�/Ns�G��0�"�'��%W:��5Q�Hjm��1@���q�V^��g�1%�,���ϫ��@��M��w��(�>΋�c��c�yQ%��m�����_��".!C���託7��T7��Ο<I~���I B�l�Y�ibN��Yԫ��{U�C_T)+֐u�hKĮ|iڵ
��)4�z��"�2,�P�mݢ�^ڪ��2Q,����)л�O�[����i/�v>���P�܈�طp���5g�W%׷ٝq�W��-W��w��y�����\0�Tۅrt��7�(��'�ѵ�(���|Ĥ0n�U�ڝʃC��-P���Y�I����pf=6��d��w
}���/ht�:���:�@􅝐[�!U_鄯z��ZyϷ�*�>޶�^/���TC�]����L7e�_��%d �Q���s���*�]�EK~�!��K�N^��Z���FD'ԛ�	P�6}�{T��*��^�,��'*��#�{�l�(�+��K�-,b�Wis��HW�rEn�sq�ו�j9�U���ߌ@&�Kٞ-m;d�5g�W%׵�b��si3��C��{�I"�AJa���bm�OHFJ������Y��oRa��Y�r��oD�_�ɍ��ƪc�kE���c����dW����*@����{���xV��H6�w�����o�����0(M��ȏ�V�q������G �c/`����3gXɼ�b���]��� ��եt���;��Z"�����%�c�m�Wӂ�;�U/_	j̜P�B���bu,hV�q�\�x��V՝�k��YooN3Y:ي%��mj��W����֙�֗���b�.t1eY��|k��jr��,��aUb�E�3�[s�}Urm��!3V&ʨ�6Q��ܟjA���{AP|_�� Y�M�ك��P%ʦ�.�m����4��όzA�I3,���%�~3��Ia�v�frA�:g'�-��U��Q�fe5�#e1�{�b�"UAj��m-��T�#,�?��U'�N
Uj/�������>A�f(`�®C>��U�0����d��ʛ8!�$K�v/���������/�*�«.2J!�8���{��jֈ�� ĝ�V���J���_����W����2���e�K��p��-��X��P�M�4�`T�|Y� �S[C.�M���?K�6��i���|D��@(֜���d�Y�U�5-v5D�)��r�
(TX.7v���e�?�+VX:lƂ�NE3āFK(?�ݽ���qoD(����^�U�
�@���2Ur/�A	cYM�� 26��ɢH�Ä�"r_$)�����!C|@VR���!��R� P���R-���'͐�����!"�-�"�h�T�r__X\_Q�|����>��b�
�5��`�=��	���/L\���}'��h�9{�P��&m\�E�����Y!'.�ty[B���}9�T^+� is�.�X��ᦴP����݇��ߌP!b�Zj��1�T�b���j�߱��a��}���ŕ�#��9�}֜u_�li���`��s���3%6�m�?a�h�_���˝�r9�mI��l�VW�f��y[���>3�@�܎�Щ+��<ߪ��������#tp��W�P���]�W�\B��+W�8B7�%2�8���O]dT�3O�{�����PoomN��"ʰȵ� �|yV9ڋ�j,-�z�W%;�U�i�|��7Q�g�⨗�� ޚ`R7Vs�j���/�l
a�+�`�.��!�Y��➥��h&֜�b~p~"�ɚ�n��񭥢��j�����L{C��W�J����^@�B�B���wzr�|�"���b1�J??�Q���_��
k�V�uA���Zͯ����e������G�Qv����C���Cz�I��q��N[��5v�Fj얺&Ԉ�H)<j$�Ġ�&,a�eY1�� �fA,,[/^�Z�H+�z�z����H��I�SA����d:������������s�wt��{��{X59�O�ީ�������)��5Q�7�������/���(w�?Z�� fU�>ҷ���gd� D��s��Cv����4�Q��I�s6E-?MO�-�7�:]�7�Qa�S�F�w�^!Sh$If��8~���-+J(�Ճ�F������樮#�<Q!�y��+I4��}�gf�G�!]�����[Vu{V������Y��]��jΨ	�38���͏4�{E����=�Ǌ�bE��C�X�����F�]�:�$�s�����Z��l�Z�=϶>����l���g7m��.Ł*��Ă
�����_M���UT��E�C�őn=^W�UK������G�J��s����?���C:��*��=�/�=1���Ƴ�:���F���}Z%P���6��>6�s�ey뤏рXC�1��5��p�ӯ��,�"����Bv���Ԟ�)j�/uly�v�"�@ў��<t��.5�n�(,�X��SZ
��sAEJ!���e�q���pv�_�b�]�/"��Z0+n͏OM46Y���{���;�v^VyH��Y��H��/�]-��6�P|�G�@MP���#���rdxy���pdIXPv,r[9�m[�I�����Z�r�����-�ΨR��.��,��<��{Φ�%����b�	��B�d6����;yq��G.u��KJ�78�!R�5�\P����^hn��vz�~���pU�`QQ�B#OG|�M�!D�s��-O��m���B��f�bKV�M�"Z�K}�{���x��B%������6���	�&Gnt������s%�ˎ��������j:�	�+:�y�AQ+$�V�k����'2ߴ��=G@"�ئw�{�Z��l�Z��W�]�^vO�H����7���S˟7�Y������֛�3?>��=Ib9�]D��f|ˑ_1����h[���G�0��#$>��9o�������yk�}��Uw*�Q�qƷj�+Nx�"�]G �(���aH
���p�����m4M���"���ģ�����h���]�z�v�B��٢?�
+�ԇ���v��p��Եd��ַ��[zg'B$���.B��h��I���Ʀ��"���g�����V���3Fx0�G����M�m�����e��f���9;4��gCUD�ܳ5��g��|�~�lP�+��{ڟz�ϨXc�+�F̦�vH�
����)m���c�K���[뎏��KC�!��8��GÉ��y�w���Q���OiionΜwJ$���VD�Q�uܫ��x��o!<��J�T�8=�i#�m�jB�{�f�i� 0�۝�]_������T;G�|��6�<t2��"C�a�΂|��,�r�v���q���3͏qKutY�۵vM�]��GH"p�٬"�=g���	IS��m�pb���ܡ"M�l=�9���"V#��[������LǼ+^���DH�p�٬"�=giɄ\�SZ
��UT:�CEZ,*�{#�E���gE��S���	2�p�s��CHZ�=g������%b �* ǽ�9�d.5�  �����D�l�0t�]���ꬱQ
ul�9�,`p�!��=g������%'��&_E%|EM̭21�l߸!�_;0l��_�-!�ό� _u�d<u�+7!+�{�f��9KK&de@k�>�իĂ
˫D���5�PB[��9Q���P���#�x]}dZԊib �s6�Ip�YZ2!��͈iw��͛<���W����
9�|�� �hω��XcɄ��?�"�}��gSB�{�fF�9KK&D����&��غƣq"�
a�	�"޷S=zZ���qh�B�#�<�|�3����Q{�Ғ	�o��m��$T����e<b�]R��0-׾qC���u��g�R�KL,�P�#�3��dhɄ�~�.�M���غe���#v��k�8h��-+G*���UTv�_��h������{�UՖ�!�d�d��̏O\n��^������T�C�ņ�(3�؄'*�#�pgA�FA��ֱz��y�c��.!��
-�dp���h1��WQ	O�qv��%����zss4D�[V�.)��A������o|D	!�h�$�����o�aE�N�� ~ A=���2Ը��6��hg��5�dB�Z2�L �sW
;V��g�m�\PA�w&���Dc��I�(<ZS��ȸ��Suͱ���#B�UВI� )޲r���cH��۷�������4jO�ƞn(���Xh4~���B=��
!�X-�d�5�g6o:��ω򸠂(����o'������"C<i��
a��#ֈ�J΂|�jK!$>h�$]�l=.T@V�Q�$�3��9F=!�g�I�z6�A캭��C���4��[�p�!�X-����=p��޲rH�ؾ��Z��E!�.i����(�Xgs㶋'����S͵�b9�d���|���[`����
�<-�W8ɀ=������4�!y�5���ש*r���Z��O8!���d��@D���!������b�PA�3��#V,8Հ�����`�;�5�0r�vҊn,�@B!AZ2I�K������m��1�S q૨���N��'?آE��
����k�#VSD{��a�B�-�X�E�S,���_\s�XxrFkj񯁋z�U�݂�C�c��Q��G{�a�oBI>�db��SP����9���]R�$ಞ�RÇ��L�ټi��X#�׾qÇ5Ԩ�������!���db$0����ho/A �b�
(���d��D,c��8�a�hl�^�GZ���P�h��i�%�b�db�o��M�=����(K�0_E���?*�Ԙ���1�l�*�1��j����g^�"����ɏv׾q�BRZ21���7�	�\�g�w=7^W?\U-<�Ù��n�,*2cF��Z������Cc��Pc���#�����L@�����>�w�?{�!���kّ!�6��b����~�+И<�����B�U$ɒ�'�8�i�+7ޱ�_�d�~q#����~��3��������U��Q��������'c����T@�k7|��غ9k�7Ek�
'�.)�vu0,��ԂBR�-���R���)��ف��6�kta�!�a��.N���*��}�Ʈ�����ի����<?QX�͟���-��!� ��cZl|�zA�	���hg�(����͉��<c�BRs-�k`
~\es^�M���i:���]����X��C��ؾq�I����;�1Y��<���M���MگB���� 3�M��K�K�3����$&.��{v��<$9�!d�I���e�1w��UT^t8�8:έQہ�B�"�
p��<2c�DK�����͹b,-�Ǿv�!��xH���!�K����"���	E���Rx��[�Xޱ�Nw'���6˒[N������!B���oT��,��!�8we��z�;b�qz�Dtq4�vL�A�bhq8���p�P�C��p�;ɤ�<�Y�����?�휻"�^����8j��1���S��!�b���:�����2ݽ~�F��s�9BHr�t7��`�%�폏�����b�38��̟�����<ZSk�rP���~]̅�I�6gA��-5[�h(�8c�o��
p����:1˒?y�����b����ן����B6�,���)=�Y@j�pU��<Z�=썬x�!)��9��,s�rHot�錙8�_�_Z�/��X��s&�B�K�ZR"DO�U��W	�]g�,H?��Lbq�
���1o9~sN{ݰ ����\h!����4�֖w2!D��n���DK�����c��'o�y���'��~�E\GKu�Ҳ����.����}��;5�E�����w�Gr�sǮ����.�O"@���gbFS��?m��+�G���lv!���PEwi�$��җ�����\�B�S��R4_��у�+moВ31�l��pف�B�oLE����h��zhW��u|c��ԁ�ݜ։5��"CLI�p��j�j*�&�k( ���n+i�P:<����F���H�C��J
���'���hJ@Qۘ��H��hB�����@��0�wz�"�>E�|���#�k�< �q"��G{��R�?*�3��v�*@ZE7��ڿ^ޭ��6��F��a�2u�;��]@D��p�J:s���vk,\�-�N�qք���s�;�	d�p�9��<�ιY$�,��׿��9������·Ty�����,�o��'��wnw�>�QM���I����$���)[�[�h���c0?����&'t�A�0]\?�+;£����)
 h��Q�@)\�
)9de	PT@�	���V(B��B��.����� ���G䃮���t��{ڴ��ڏ�t�/��Z��Δq�eE˧u��ˣ;�������/�D2��sf�&�ؼRĻzz�7�&
|�ڛ(���l�yڄ�D�ȓF�`#?�Ӧ�H��.�?PiO��L���N�*��F��F8\B1>�|�u�3�U��}��������DK���rǓ�{v���t}��A�s00>��z��ς�V�c����E�����{a)�\���"+�������� ,y�)�}�%�������T�t���g�_܅%K1�h�<-�#�Q�r�h��L\�Rj���E����)�#yd�**�ʋ����St�_��<2� ����{nZ�����p�T���F@1�B�����ꉬ-r�J��~�?o�~#$�cɕ�;aɯ��Is���=���4�Z������B��)�\(巐O��b
Z��;�~Xr���(��H���&Z��\(��� �H�G���<xD\+@8vlvY5��������c���p!��YP��p$7��ET49U��
��5��"�*B*��n @*q-uBP��%�d����㢾�w�1S����6$�����#EdE"
E#CT+/
��5�m|eHu�jc���B�:y��*�J������ȿ?���*��҈�lw��Ӟa��	���`X�Q%�����A��jX��M�Dc�[�����MNiR��_١���tj'<��Q̇#!�[DV��C���r�R������H����Y���Ѡ����c�]�������1���:a�=��&Z�ԯC�4��K���x��TM{j �l:5�����	���&T��M�"�;��ל	\�.�0�Qg<�=��T�+UI�
����@r)��3�;_�O���љe��H(�p�w����E(8r����OP�V������Ϙ�>W�"o��L�؞��GӇUǒ������/�Ët=��]k�������b��zv����G����Wi�A-☽��7���<�4�+MG���ک�g�o���r�O>�����oG����gZ����y��{����[w�42����H�Vi9�Q1���b�o��*��K��w�f�^�U����<aS�}��Ka{PLy��N^��n�mw/(�"��_sF���0 �~�������e��(Q\K]��������r@��]Q=�p�H��Dn��_=_@sЍ(N�.Ph����%�f���/Z�DKr��3�6FwUS��_�8\���$��t{������V���̈́F�=BR�h�݂�&'"Զz�	jx*�S�(��#'c���>y�#/v~8�洵���K�GL�����ը	�C��V�V�ϟ+������^��b�#S��p8��	�@@FU��.�>��T���A��5�-D�T��mp񘖌$�
���GD����x*�=���[2�+�JE' 2��g��_�e�zJ�h�$����ک�:�:���@|���� ��-H+�B�h�+^{憏-�cɁܥ%�5b�h�*�`x��͛t*곢E�<�ָ۽~����BDc�������������Ԙ@�EKW�w�H�p���v�w��!D��[0Q�Ē�D�|�#r��b�t-�c#s�]�M>��h�!��7�u=*�=��K!m����{�w�̌�k��<D΃��F�"��nx��=Z)���C���|v�&2il_TC\#�"�F*��Ύ-}��' h)*����'l� %Aq� ��@����h/���فN�j#g$�>"�VB�D *� U��F�J���9�C�������}/�V���KR ڈ������p"���*��Ҳ��lw�� ?�Fŉ�����7^Ws�q�H��E{-�vB���^��Ā�ϕ�3#�|�Mqw2<��nߌȓ9�g�q+r2\���=q����6I�}�x���U��Dݠ(�8#>ʇU�U�<���b�#x�RH����}p>���?{�7�,�ЬhI y�5:�!CcK�ݶ뮧[Z��D���}o��5���E�"C9/��Ţ>���`�R�vg��|�?$R�P8q-uB^m5�wBd��PJGDZTU.��_y��TR7J݅��pUP+���\$D�
�F� g���43ZrT@�0_�h:�:P�"�O~��+=��(������/-�V!'g+����έ���d���%%1�A���B�{��M4K�LT,�fD-}\��j�ê�Liܖ`��*n�>Ō.\��}�ş
�{��ih�"-�W����N\i����ˏ����q��w}�����׾�U�<	�>�w~r	�;����=��D*E������Cv�+�c}�>~�{��!2-
�"uB���&RL����&�(�G�7]=dYJ+o�v#}�� �Ȣ���ɢ	�"�!��q�.ɻ��	���4܊Yt�c��o�Yq�k�7�?����j���K�B��z�0�k�}�$Fkj�7��ݡ�1�ly�!iA��Ų׫&zv!��h�ݍ�c�T���G���8<���s��\d%J���-����iUy�M����<������P4���OC߹���q�ޣ����'�DX���H(�{M�䣚%v��H.�P�wzf���܇T�CA�Zq-uBN���H1��K1ot��nA��|������%)��9ڵEr)�͏4����F-�ME�����·�S���������c:;�p�}��S ?�j�����-Uz��ebY��fc������pU5\V��p���m�V��.7��#$-�9��|�=�|�R>�����P[1+���Ǡ��Gܒ&�U�O��D[�_�W���3W�1���EL$�"-�z�Il�y���T�#m�<���<6�
�C��A��_vj��4N\���y�]f�UM���ӵ��>��S�P	�(e��1;Ö,���@�+'�DM����lyW��/C�F�P��}�R8Ң����֝U=���O�#�G�1���@���dy���٣��\߂�@�Pѓ��,mj��w��W ?~���5R��_Z� ����I����te��ۚ��+R�gLEF5`�+Z�A���������'lҼ�U-?&}�Bz����V�����R�;��+��G�������!�Ĵ6bFN>�3T4ML�K�Ī���ľ4����Q1��	���3���saY
y�Ïg����u���z����@��fO��.\�mW�󩆣���E �+opF��"�/�]-�6�S~8��8T��������	*_\}UI�/%D4QI�
�R82i��#@L81zL�~C�*2��Q��J4A~�iގ��&�j��z_��gn���Ѿ���^�3�}Z;Uz��e<bYhhrJ�WU�w���h�2��/2<�y��#$�О����#K�K�\4�_S��VLwG�麾h���CZ�:�C�^��c��h1��4��	!�=�޺S�Nsxŏ�y���t(�S�����RH�A��~��5�q}��w�{�mL�
6Y��G���P����C�>����D� ኢ�-*����S������j�hTL�B%�J������DH�)?.�T0WyW�'��>\�y�yZy��L"�J_�CϨ�-���&�j��-|����T���+�J�� �_)r�W)���Bz��e6�۾qC޶$ld!����t�'�h�{��I��X���������ë+S���ȹSAѾv=���P��3�P���|�,t[@1�.���s�%&�� ad������+~T�{��C
������W\?z�c���K��'� K�W����h��>��Q*�T ~Y:���<���oO�ԇ
�kq��S��M^I�;��FqUwF$Z�#�ڥ�Jj�Α>�u�.QO*������Ӑ]�����8;�,�A�Bm� �UsƏ�h�l�ٴ�I�*�"���2ሐc8e�
E����@4wI	j��Qd1Bs��x]}2W`BAc��>�PRkWL]�'o�s�r������Ŝ�F�ȩ�^O�{j��W�������cβjGИ�|�%�V�Hg�<����
)���$.^;�hr�>��#q��[�g4"����|����T��A5ToA�ъ�j�l��9�6&/N�]�"����[�ǌ�'�����C�#���2���1��̍�e役9:�u@vQ���\t8���GU�=BҎh��#ᡱEG"�.哷�H�,�|�5��q$��1��Fn�K�W�wW�t��mW�*�β�'���ʢ-Wwi�[�߹����wΪy`�,�������!B̀�l9P��z����P��
O�,*ZQ)�﮵k���hl�{��#���bJv��&��4uiwq��{j�F�����˧�U��Js��:UwF�&J��<z�~�m��o�Y�ȹw8�Q1)ߵ��4��[�R$S�t��xG��?��lwOonN�W����_��R�?�Z�����t4��Z���Nw�>�6�z������{ڍ��6g���c+���tڜ��1�����G^�{�!B����g7m��,D�g2���a+����_�,N��yT^d*��\̘C���y�,�.!���n��%���:�<f;�bE{�{��I��~����?ֿ�Q�D����Cs�#+�'Dܱu���DO�I^�M1Nw[E���e��+���p��"�X��/ܵw���?��k�$!�GCC��������s�t{��&��2���<�NL���M����9��b���}�'/=���'K���ǧ�����L�okF��Gm�"ǡ�_�o�h��T�{��;���<�NL�d��ַ��[zg'B�$N�w���@��9Y�pUu��U�B���7nXѨ�E����	oY��͛��᫨�{�d���<�̵dp�1�����u�G��!+�q�?N��h�{��(rr���>\�$!
Gkj���U�V���=��/�C�t7��`�%���ow�w}���O޺S��GȊ������C'��7h��8w�SZj�2�ۚW��1W�Ǒe��o�=B2	Nws8&ɰdBH�p��В!d_E�J߽��8j;����S���@2!���9�-��{ �V���8w:ZS�"����i��x���$�󎠔pMI#8��y`hɄ��.Iu�[2�,N*Y�B�ñ�M��EB=�8��JO'!��В	�v�r�i0ѕ�1^W�vb���%���$�M!$u�%��WU��m�d9^UG_�[q��5"g��C�|b�3��#�����LH�=ul�baFkj;V�Z��m�VXr�8w�t'���{���В	�F��!ò;T\�R,*���hgA�@a�κ�I|��=B!�dB���hM����Q�j����Ƿ��%�|c�߾�B2	Z2!ق8���!dЛ��]��"�lw�O��e���|��H�3!��̆�LHV 
�hl������+��!�q7�{�:�?Fkj!���BH��LH�p��l�d�2=�s���V���Oi���%���kQ!���dB2�����Y����!N Y�(���"n�������9�1ԄB�В	�L���{�	���unQ,�Ǎ{F޵v��}� �(k����"��:В	�@���y�|��W��,ȏc����<Q�d�q��;POkWlBIAhɄdb9��[3j2?>�b�9��:�W����Ww��Y�L!$S�%�9�/�֮�|r�g��q0��w�:��Т�|c�BH$�dB2ȥc����͆#Fs���	�*���sW�ǧV��e�v�X�c�BRZ2!i�x]}�!wI����z	�*Z��vu΂|�KMĶ�ԂBH4hɄ�1�<Oi�Xlye����3�7�Q�����ի�~�,*Z�����q�TB!$�%���**Sgf,�7�c���:wmS�Gkj���+=%�BH�AK&$��ܳ�=��TB�7'�o!r0�\�c��DޟC+��t��X�i�BRZ2!i���Z�"C����w�]�+w�k�e�g��A?@��K��$�qkB!Y-����7?>՟�-u�9��F��	i�<�a�H���g�BT���~�Ħ���x��O|�	b�Lt���p�Y��Z2!�X��:;�.�],*��͉Os�e�+�D�A���Qh�t !$u�4�����
�v�����]X�m�:]����o��n�?o�׭Z2!i�hMm޶Y�+2$��p��D�v'V�z����=B����)�q��y�7!b*M�|_�k��S˿t�В	Ii|�p;˫!�k߸!��8��q��'z�+Rd$A�S�g!$E�4�o;s.`�Af	��{ώ\����-����Y��RC��?�s��x<(r�������8�������R�6�B0D�F�鱯���^�dBR_E�x���ȁkB��E�G�KJY� �[�>nH��&!${h9=�����H��s�ն>���В	I-��g6oJ�Ó����7�'�g�y�WU������R��GQ�}�^�9w%D�����G- bBK&$��G\�k�M��VJ�������
W�d��8��7�!��폏�����b�$����Y�~���В	I	Ķ �VY����q��['����J���4}��#���!��'o�9<�X���?a�Z2!���l=��&
Ļzq��o�%�.qtȊ�Q�7� �d�K�C���K84LNiɄ�HC�)�*@��6\���]޲���
t�_�"EF��X�"B���]\����P��w��2>��y�v~rI5�;��7:�T)}�~�s�4
z�/�-��:+�����������hf	W
-���o��0���8/�-���k�{�lwO��5+:��W��!$&�[�ƃG��.��m��k(��f��V��մ�a$W�d�5��MR��R�r~M��A�%���,YѮ�ם�ޭ��6�dB�
Cȉ����pUu���Ê�^і��z	uX�^<c�����|H��c]���>��9o���e\����=mo��q�wn�_٣堊�]��Td�zḫ� X2��h�"Z�hM���?y�N��#+�}�Z��}7/���%BT��"�f0?>5XT���y�o�8�z��c���U��9,����63R�{a	J�ȋ���1#�w79!�"����o7�#���1�������p!�'m�V(@Yg<�������Sb����:��"D�h�
��N��{nZ�����p�T�dB��@!��E����A�Y���-^X�	1��j�LBR���\(�v�W���gZ���]�7i
�."h$WE8�FHj�gA�VoؒUou!_��0*�>c���% ��ko�	�Vضv&���ȿ?�����L�o&�:V�J�U���7�4���'[�w�]��~�W�J��<ZSkyOB���ԯCT��7��7�|��a��}pG��N�ʏ��.��}�-��s�{A5-�qWgA�aɧ���<5@�T ��>���aձd��j*Z2!�*�{��X,��2�WUw�_�H�T� X�ڪ�ӟ�mEgPн�(>!$��MB�x�N<2���ɱ�_s�_�[�~�{a���o�ۇ8'?�����@�_h�b
�;O��5�Y�����(
�����\�>�]�
ˁ%��cdA�P���={L#����h�1�����L�zF*!(i�GO��f�`He�sb��N�#!$ˉf��������6�/�ʈ[0�ko�	�V$4Z�Z|�m���R�GCR���H�a�(E1���h)"��Ǘ�]��_��C�� ����[ъ~�>
���%Zp��LQ2?>5��3^W��Cȗg�5���D�I�����%>��6:m�/N�wt�]�7�!+�����Fg�� .|�����
��}�}��ADSpvl����O-����S��.q���ov�U�FB���[�]�[�&"!
U�UL��E}�h� �F��6�����]�T�dB�_E%�-���B��7ı�A�X@l��޲��ܜ8�֘hl�{��8��]��@8qd�����>�����G�/����s�N���������n���ǆƖ�%��>��z�tؒ�+,���6�QJ��?d�۝\�����f�ԲF��'?���2>J�j*Z2!����p��� ~����5�2~[s��u+o�x?BR���Ő�k������3���eq�����	ۉ��v*Xi�Ђ�-���-���¿Z<Ro����G�(w�����[{g��ᆽo����	u���ǿT�f�ͯ��T���|�3��hɄd.?0��g6oJ0��j�![�M�w��+M8PX��X8!$����φ4�+\Yl��ĘvZp����m�ǐ�����I�s�kA��qW�J�;D�krv���G�;=3������'2-EFλ^uJ��s̪J.����|
��]�T�����%�]�mͰ��GO'XI(2��E������=BH�@��fC�rb(w����٣�j`d����9|̇�Ͼ�%�[�7�=�rο--l�ӵ�z�3lɪ�]wۮ�m�qQ����2�޺STIp�\zP���n!�{j�
���n����˯ ~����k��%�-�**�7���A+��;@�v;XTԟ�͐Ƣ&q��5��.%��5�љ�6�͞�EG>Y=����QPv,2&�78sj���;Kj�R8��G����}�V�8hn�뮗����d��6d������iB�q��!�D����.����c>�#�/�]�����^�3�}Z;-����Y���C�sޑ�ܜ�ƛhl2J�Q%��"��pk��GI���t(&�����k\��n����e���^n���P�<��W�Pm���V����[r8�aɊ��9(��>#>"OEr��~��]Dn:�Wm#����N��JqдMۛ�K��S�V 7=ݥZ2!����[Vn�f�EU�f<PXhTc/��ׯ���At{*oBI j��!vwN)z�q��{j䷠��ʳ�"m��t���Yuw5J���KQ
LD�~ӝ�P��ppr`��ޒ({ŉ�Y����mH��&�z>�&����m��Pug�D�%��@��lޔ�C���jiwII����H�ć�%�v�%-~�BR��o*�[�gN~��zk��><��O�|K�n�/R%UP��N���?Z2!��x]=D�Z^��WU'�8�|��4j7	䆮�om4��غ%��B҅krv�Ɩ�O�H��%��̏O��mK�!d�$j뫨Lp�������]4����q$�X�7n�{��X{OM�I��ʘ�t��o���� &�dB�S���wZ^��@([�$��{��4����o0?K���-�XBH&qϳ���h��C$�|���/[� Ą�LHl�!�t��GU=��	fEF�'����hM-�=���U��X�BI#^8����?D�Lў��<t�� &�dBb N�H�!�`x�2�����'��ok6�b�T����KJ�;2!��r�'��!�4��/ܵw����~LhɄDE!������H?:V�2p�=��ŧ�0u$O�Q|BHz����UwW;���!������O^:z�c�W�Z2!�@˺ׯK�!�`�D!��6�z���i�nk���3>�EZ||c�b�m}k�}��'pv"DL�ϻE�~���/]'�dB��!��OrN�g⇆���W�_����Z�&����<c�b6'�_��_P�Zw|��^q�����?����ڛ.��Z2!���,�����7n,*J|M��j^k`�[�ķr́� BHr��vg}�����;?��'���KѱO:�k��В	�=��S�\���YF��.k�o8���<nww�u�	!��dB�GL�!�`����3�6��Qd�qonN܋@����h�=B!	-�d;��S͉Ʀ4B�Gj���x����ص������Ҋ�|��G!�Zh�$����X�*�����M���4n���3n�F®�k��!�����L����)�5Dzm��j�ټ	�l�j�qon��[y@��^,!�i��=B!� -�d#b�����E��l�D"7􀱊p���q�i�؄BH"ВI�1�zܾqCz!}WO��p�[C�{"�뫨D�,�gB!D@K&Y���t�9a�;ұz�!;��-����8���#�i��7�!���d�-x��?2#9xJK�:����BF�Ud��غ%����Ʀ��'���ВI�3^WE6\� *�,ȇ��Ƚ�9��hp�9�C���M-!���d�������*�`�U�9��(��O�5�^�.�
y�!��Ԅ�L2�[��ƿi7���.D��BF����Dv��<�"BIMh�$��C��
9Vd����a���S�j�D޷C���-�mB!DZ2�4`����
I:+�Z��Dc��t�wH"�7.7~	��JB!Y-�d�KgA�}�4�PLlcܛ�c�"#�z�C��x����BIeh�$C�<*.N�!�`x�����!�]kטa��-D�B!f@K&i�x�����I��o�`�nhpP`��r|��j";�!��-��c�BH�@K&iO��u�>�l��d�q�αï�D��Ş͆l�L!��
-��+b#��9���GC|�M8��{@��nz=\Umy�B!z�%��Dl'��C�������}�s���Wtx"6�3����m�B1Z2I3`�C��P�t�Dl���Y�o�@8�{�:�ފ��Np�foY9!��FВI:̀!d�l�6c���C�Pd��Jb1�my�B!��%�� �6���J�!d�A���s}�flg���v	�ۇoOK&��^ВI 6m�[^���-	n6� �bޮp�rܱzU�N!$��%����(,L�!�`xķ{�:c׊��9&)r޶�"�b�c�"BIGh�$uC�Ǝ�Z��5�����X�Ò�ıu��#���ВI�r��oܐCȗg0E������

;PXh�[���	f�)-�{�B�Z2I9&[�w�_��g�H\nq4��y�;���m<<\U���!�?��_"!��섖LR(Zf!�:;ZSk�����(o�6c�[�!�._t8;V��/˿B!$nh�$U���2���@�����M��F=�_)	*2<�m�oB!$�ВIJП�-c�����,�cS!����m���7d��Ɍ.	!�d9�db1����g�M�1�|y&���e�8Zϼ����5	���%%�uB!Ʉ�L,c~|*Æ��a�C�ņ��غe��֤j��	�>����g�B�h����;������B���1�5�M�4gPr�����3�!�d�d�l�e�I���4�8�ؔ��@:Yȷc��r�;5|6!�b-�d�T�Sp�BF��ׯ3��Q�)r0��Ő�o��G!$�%�$!���p������l����3�7�Zs|��-T��L!$�%�d�8w�77'Æ�aƎ�[����ܵv��k|�]���:�.ז�B��В��@%��p��;��l�xs�X���<?>5�ؔ�72���3�!�d*�db"��B�7�𖕛���5�����8А"|�<c�BH�BK&� �t��̏Oe��`�U��W��ǳP���f���!�����BS�J!�X-��DcT,󆐃�
h�k�i��T�?Z�݂�@��"&!�"��L���L�ok�n�Ș���M���9����S�n�����EGf�BsB!D-��ؙ!�#*R�G�I���w���	��^�.�3���7�?_�BIAh�� `x`��8󆐃�w������R�l��|5��S��N�|`��z˿B!�lh�$Q�r��u #�X�ʤ։cVLUdd~f�њZCrs��� B!Y-��,�r�7n��!dӤm:��� �lE��u�	T{~|��o�BI�d'�u��We�6�/!�&���:��av+ �F����{�:��G!${�%�x�>f�2,ֱu�@a����ܜ$���)-5j��9���#��mВ�ʘl=}��ʼ��NH�I/���Z%��pU�Q�f���9����BH4h�de�r�o"���M��!۱i�$��V7i�hB!$��%]@��;�o�!����י�@d������5�?�%[��B!ɇ�Lb ���!�`X��X��0i�EAF�'U�o�B�Nh�D���x���<����4gA�c��t�ٵv�!�z�,M0J���m�Y*�BH�CK&�HCș�I��S��S������%A���F��=B!��LT�"WU{JK3x9h�(/r��OΊ��1j�|�d*2!��,��L�b9^�
��f+r��UIE���v�8��.)1�>B!$}�%��AonN�!ç�\t8M��?o[^���xF	��#�B�dr1�<\U��z�(,<�y�y-�h���4���D��m�I�{B!$��%�߯=Ȇ!d4
8T\l^K�����&���C�j��/kB!��%g5�gPF�Q6���"@OWU'G4Gkj�:�:��pf�&��G!�HВ�������k��2~�E0��/k����<����@7u;<B!$�%g#���&q��Ih,�l�(������]m�Q/�z8ZSk���BHf@K�:`�b��$����U⍷�(�8��2b�=�r[�B!)-9��E��d9�IП��<;f���������pU5!�B"�%g��=��|���$9�yGzss�"���'M��"���-PmgA>7� �BT�%g>b�{���B��:�9Z�B�/��6����60ϡ�b�Z&�B2Zr�#V!gժS�r�5�q�]2�v�,c�iC9�nɆ�M!����%g2ℋ�B��cC�M=zZtl�Fn�����=�KB!�-93�;�VY5Xy���1U�џ��[̶p9�qc�>�3���!��-9*.ζ!d�+l���U��t�_��7 �g6o2�Q� B!�Ą��Q�v�@��VY5�p�!�f�����i��}
Fkj���*2�̪g�B�Zr� S�m9^?�_�M��"D���<b7��`X�{ss��)!���В3���X���$ۆ	�}PI�����f��|��K9����ȄB�Nh��Q��U{�	|�f=��/���v�uƪ����hH��#B!$}�%�1P�%Y����-+7�]���M���ի�]6�^:�y�~#�BV-9=Pl=&V!���X^����o�`�����̵��Y�o��諁��d��B� h�i���̩�N>��غ�mC�oYy�CU����a�����q�"	��BH�AKNz�������/�|�7*N*�N��ټ)	A�;V�J�(2�P��%��lwON"$�B2Zr�3k?E���>��,\�,�UTv�_��%���$�� ^�,�76O���t{G2B!�d��TG$��~9�����sW&[�������[V����<����?:�EE&�B↖��H�WW\���������k�j}�;қ�3XT��������<��B?�:>�����BHVa�%wNn?pb��Wn�c�'��I�o��w%K�/������z< ���1f�C՟��WQ�����H��,�7���=B!$q���K�Ky;l����g���<�х�߆H�� ��(���O���q?T~[sr��
J���Dc�᛾�몧�;x�!�� Xr��������!M�|_�k��S�8*�^rv�p���mK��+D֌͘!�跬Z�C!��D��|i~	&t�\�r'#)��E<{ώ\��D�V.�hMmTe�v�L�O�������=B!�@��;Km/؜�!�������t>N0cx�Pqq��3��-�)K~�tz/9k�	!��l !Kn9=��������oT���<Q��9I[�,�Oںg	�l��uf,G����B��$d��;���ι+!B4x�֟����4��᫨L΂�9��ҒŻ�5�޲róE�A���!�b 	Y����ȫ��_/����3V�_�A��O�)q��63TU�Ź+��&�,���B!ƒ�%�֝��K��!�|��OD{��ǧ����p���SZ�|E�x~u0,��y۸�!�b8	Y2����P4�Ƃ@#B
r�9w��^���r��?8�G*��H'�Wh�Z2☴մN��-����yG
��Ic��(���	!��l QK�����c��m�û >>����䒸�e������.-�hO��V����M��k,�-T�g����V��ƃG�:�
*_w��Lˊ�n+iz�׿�T����0�9��+BՒ{ss������k�3^�����|��֌�!����B�̵dH�ܓ$�����O4����iy ��z,Ɖ�/* �(:�}�wv��.���;#ݺk(��H�ܢչ�%;�v�s�Dq����{�`�~�D|E����B���R���B/-�
^9�C�i$y�����d8� 9O�� �x��x�����&�1�����	!��HԒg�C�8�qՒ����w<e�lrj���OݶK�wn!Z�m̠���i�R~5���ԯ������VR�$D*DC�Gk:�RA@j� |p4���8��ùQ�hm,{�O�"����U��dyͥ����ܷ{��I�*�<Q7���G�p�����U�u��ˣ;������[�Z�f��)9��(�l��Io�!Ϥ��H!�d'�Z��\H�����c ��:�����#P��'m����i����&�g<�%*J9#>�k���rF�����eEx�Z�������;Eʂ7�j����ro��(���#������o���"&>�k���>���R��+����o�iy��F"�USI��8w�77'i��B�-�Ij��zwI	�	!�SIԒ��B�4u��'Ö,�{Â+E��V49q��H��������0�krvtD&�.,���YT� �{v�"�Ȅ��
G�Gk����*n�;_�C�caƵF*ws�>��9�*r�v7����v�<������^�DAs��>���<T\�L����yG�f�r�2h���WQi��8!��=$j�S�E������K!���ל߁˾�D �r����O��	O>u�.�#"\���Z�+��ת�J9�
�� 5I���2��,+ni�	���y*d�� �������v�#�}њ)�qU����f��v�彍�Ƭ��s��h���X2�qW5�����c�gA~�^5���� X�u�&-)A��l��7�!��IԒ'�h�v�%���{Xp"������O�~�B{dB��M�Ǜ���`s�Bd�|��֝�tF�9�S$�Q$��% � 2h���m��#���G੨�[�~����%4H}�QT[ �42�-�w�f������*@�� E��hI�����h�nd��>���&s	��٪��.�zssL�sq$
��#�B����|������cB%�!P@سjB��dϰ�krv�_�%h=�h¹�9��'D<ҒAa���k[2
��G�E҉�]wۮ���(4Z�%*��EJ���'N_02T�SX8�,~l�MD�E��מ��@��Xr�w�}�Nw�����K�3=\U��dY��6��4j���k-!��䐨%�/�"il��	�*�#���Nմov�!����o������<����q�
<�B;�>��@�xj�m¿��[��فND�{�'���-�8�BQdI�5Z-j�h��JG�"��vg@xՒ�.�vK4���?h,ڨ3a�� j��|��)�A'h'l�q��'������KPd߉4��3���bx�U*p�=��f��>�y��#�B�F��|�RH��PC�֋o{��R�<2�>��L�|CcK����?{���}o���UK�#Ϲ��̫�c�5Ar���غ�(υ-92C�?8�E}DS*9_����珜�
D��]��G*K�2y�=�vcp��ّ�u��B��$A��Ԣ��%�9�E�C�Q��?��#B�G	ܕb:���������%�i��pB%�RdgA�y�J�%%<c�BI&�Z���P$�C���W?8,�#�Gw��Lx�ŃT�����~���}~rY�6Z�1sFMD�����B��p�Q[Q��������>�`w�K-��C�/~�Z^��7\��un��n�h
���5��B!�����G���w=݂�����3��͊�_+����?=��gg���g������ylxQj��ϱ8�z��Ǫ?$X�c��^��n���{�BH2IԒ�gC�h8qՒ����[����W�|�#K���_����B�ʏI!]��E�O���=�¿�u����hõT�ꃴ��,Qj�X�]����i�}�A^ڨ�8ڂ~FZ�.f�7:��|ӝ�`�R ��vU����K>�㮆����0r�Ұ��?}|��ʛf�C}��ۖ�4"+ K6i�l�f�BH֒�%�͆��Jؒ��"�sAx*���W�"�����o�\=xyο,B:Ö�����=G]0`$9��e�m�\�&��H<���p�6�A=��}�T[���F��ЈS��]*K��� >�@��]w�Q�-&z��vt�X���T� ��@y�Q��S��/����^��ގ��[��y�td7���M�#&���x]�y���M-x�!��|��љP4^~��%��G���W����H�!d��������W�m���������빰���1����?�EB��	rӨ-�@��p�6��}�Aj�����%V�����c���+� �qӝ��>Aۯ��΍EGz=����n�H�Z��vq�p�ax@��{j���D�O����>�[����⪡�V�n4��ۮ%s�9���;V�
��fd�8we~|��L!�XB��<2�����mc?�۾��9�z�b��=���Ww�q�����^{������فh�eǐ���"T+#@�S��>���u���m�	�mD%�qP�Mۛ�����# .P�Ȃ�6�T�|��.|DY�@�HU�J�KD�Q��KR��f�՝;Z��h����'K_�C?�����������_�?#����\ �wͰd�����x`�t���,*��u�BH���%O�"�^�f���R B.�O,�e>'��� ��"�|�(���j��u��B�j��D8����<	2G���}���1��S$<;��6�8偵��UwW�5���N�H��hfd���?�or�|O��?���:4-Z�E�P4ҊEƹ��ݸ�� rd?C����Q�\���������|��b�8�[�w�m�V��@��ׯ3o?��G!�XK���
�24�\��'��h�uzf�I��H���w|+J�6>����٠�-�٢5e���'G��%y�T4�p7fݐ
15��)�!�v~�?�'�z��A\hD3֒�j]���N�
@���;x�!�b!	Y�59;\c��'C$;9�>Ա��v4c-	C�p-�����y��̻֮��B��$d�k�i<��Ո%�{�]=�ޗb��t��xG�!��E�s�������<����{ssFkj�j !�B	Y�=϶>����lc���3p���i=��}v���X��]kטg�13�z�� ��&�BR��,����-����C$�8���_�x����E{�{����T�q�`��"snjA!��	Y2�ʽ/6��{.�H�ଵu߶��^���]��]{'/.&�A�-<7D 5uy���ˑ	!���!QK������������l�����q+�՟�;��o�䥣�<�<cPd�y���[Vޛ�c޾o`��v����6B!DN��������bKO��D�d*������}Q�>�"y���D��Ź+�kY�g�+�h�c��"B!)��N8F����������ݽ44"�ćmC���v=�������������&8�<ZS}��/D�d�z��@a�Pq���$�B�c,�����k��~�֝���HZ�5�������6<�3> <O:��Zd���ړ5.:��W�:�=?>�,��{�BH�a�%��d������ ���S��������̹�!���В�:0TwI	L1�Ü(jnm��Ԧ*�8c�o�B!�	-��p��7X������?o����(�7{���3�!�����L��ao�MI.wq�
��[�H�ϏO�mͦ���� �B�6�d�?��7nH~�I8�Y'��ك��1pf�&��G!��2�d��X�����2u�%����S<c�BI}h��*�g�u��;��(�Y��
�.:���=����4��ȄBH�CK&W�;q�%[@�{ss�e�w�����&�c4�o�B!i-�\�y�u�5N���Z�~[s��uf/5A?�=B!$]�%g5�M�y�,)ZlHl��z���噀����X�}!�B�CK�^<���T��P��ˍ����-�$�A+2��#�B�Zr6�8we��g���%�EN�z@5����K�{�BH�AK�: mg6o�j��UMe�� �G��%��^B!��Zr��غŪ�.w�n� ��0�j0PXh�A߄BIZr�5�KJ�z�l��I�Z���{IM�{�BH�BK�`l.u��O�Kr:�n�HBM.���|c�BIShə�X뫨�jW,oH�Qdq�٥���ԂBIkh�ձu�Ъ
x��'�,��hM-|��%<c�B� h�t���ޠ���RdY�|��f�"��^ !�BL�����v����[h�P����$X���段k���cwI���%�BH�В3���&H��{���SG.7z#	o��=B!$c�%g �sW��PC�J�";�nI�Qd�1H������ B!$3�%g���m޲r�* E��O46��&�sޑ�c���G�	!������9�����2T�GO����kb���·$	!�b8��A�+�nﰰ΂|��Spy&�5'gp���)2|N!�C�%gb�Ճ���ԦȎo�?�j'G��˄��B!�-9�'�Yx�������#Ae��I(H���7�!��̃���[~��`QQJ)�hM-�=9�<��<c�B�Hh��8z���sޑT{e�ޛ���M���ԂB�Th�i	�~f�rXԡ{���z�{C�Ù4E�UT�W
��#�B2Zr�!x��]=�hMmJ)2:��m�O�B�@2!���В�񺘵;�AF�7��0��吜W��m�)�|B!�-9���v�X{��d�q�5=X{r6�����D'�B�В�q�4�V��#���;D^��ꤍ���ႄB1Zr*�����G�1\�SZjm���%)�W�N���d�q�ȵ�BH6@KNEƎ��~�xw�Ë�!���BQ���my��q��$m�f�)�#�B!�AKNEzs�	K�����z�k������L46]�	�� .�]�"'m�	����w�AQ��������;��3�ܧmL�jskL��<���Ĥ�6����&��&�T�C�!Q#FD��D���������E~���,��@���t����gΜ�=�Xس�{�5��|����=μ�YX~�єp����ލ�Hf-�g&zGu������X�����dk~�DDD�7L��>r���B�����U1��������ʃ���W���C�DDD�gL���?�����ܟ�*
2��b��5��&,, �@�D���'�{DDDS�8��ʶ�C�KBOܳ<��'6����L�=ߋ��������=��y��_|��2ޝ������7�v"^z< ��.e�Z��ym��/�?ןGF"�d��[J��
��dU�{���YfSS_��]4I9�[���վ�c��� ����{��c���z���,Z�ϟ8L5��gi�q"""�������v��:㵿�hR���Q�t�丬��c��9fߟ������=~�����#""���!%w�"	�:4Ox�#��W���x��҅�c_uc�/�XW�1΃�~���������O"""��8��[u�uƾMj_w�;����������^O���X�֟���_CMDD4������zb&�nkwѢE��������cu%cx�z�ۍ�V��OL�;����h����f����z��h���q�`޼�����~]yP���>]������BS\<�c����|Mɿz+���u��&�sk˥¶�	���U�OW��eӥU����C���g���Zр�)�����~MF���y�,����^�=�yT�򱟿�ĸj%?�LDDD��)ѧ��˛*� �de�}�_P�u;}����+l:�lX�(/���Rrep���q����b�Z~�	㐒��\�|�g�k�Һ>q�fw��: �{�qVen}��K�ӥ����Nѩ#[���N�\*��OD��5�E~�C46����q�_^�����a���a��|�f�չ<,�;�\c��zwLg׍G_K�Ŏv�1yJ�`�����ǘ���(�MxJF��$)2"ة'B��xGy'R/:G����Od[��e �K�4���:��ho[#/KEp�"rdJ���aMl�Ր�=8D��7F�Xp�7q�+�v\�J�GDΝ=?����o*�}u�G�|I��ǒ���߀�T�?�A��ɍCJ��uys6�fJ�僗�ۓjT���3�b�%�}�v�*�c/�TM�S4ޏ��"�H�YLUI�r-]��s���f�a�:� �c:��5�L�0�����S�v���R
}f�x9Ԍ��=����K�ڸd�V�7���<������/E��ۥ(5`��[�13�M���Y#I�6]Z���~�����~�)�CJ����;�gr���5{elt��5qu����˷���>W> �U�1��bs����QE��u����C�ӟ��0�鐔���a�Ұ�i�Q���t��b0Ff�ڏgY��"�{���)����F�xr}"��\��&iA�ġt!/nO�xsjN^yv��Eb�t��x�r���p6G�;��q�HRrMX��T�� ؑ����܍CJ��q�K3�Rs�[�R2pe(�J�S�R�h\m�s�ԮX�5�x������5�"���7U���D~ł�we���>5`��,����,k�S�;6B�D?R)
C[��p:�Cn���b
.\�B��A����Y��)n�|#�9�d����=#��n��q�~�Ӣ~����78�q�zJ�*5�����"r�g5�GHDDDhRr��.oRs���%J�7�[��7G�N�G�=ml�;1 .���s*Ho�!E57# �!����XY*@L�"��;�ar�w-ݥ�0q�˱�A�t\Ŝ5q���yƆt�����?NWԉ�P\�����1��+zP�������d~�<���m�u�������o:=���~��8K%%��5�Ξ����8�a������Q ����pys��͔����e ��#<�Y�=��7�B�O|k�����Eǝ7�aJ�b��G�eg��\L���"b��D?*�t1W�8|Ub�ڨaW��"�!cG���d!1�+��`\�4��2�,JB%b��� >�5̓޶�"/﹙�����]��[���#n���½mz6��o:Oy��g���S�~�dpW�ѦK����	O���"������DD7�N�FF��0���)O�bq�ˇ�d���d��"�zL��q_�a"�a��"�u&o�(�Չ��@>U�C����?,\�(r�~�~�4��� ��T�9\�ԢB}��`y(�����NwO�s/����8�=���H�ّ��kvG�3K��Y������s�5��GDDDkR����q��ͺ�G �J���8��)����?7��[�h���q�P�'_�0X1]�2(`�~=��\�_vf������V[�Qf�ml}��]\^?��u�YX�a�|
zڝ�=gu���ԉ�4[�S��F��n�䡹#�񈿢�"�;�'?[s䤵������D�[��"�"��S����/���8�=%��\/��?��Z��w���qHɭ�.���D�Wvf�`A����v�2��L�OK��m�h >o�
�R��YW�(��
l��J0�*� *T�°߽��̊}�}�mя܉�I�9�㔴�g�_1���,":�Ʀ���w�4�)-��(R��@��P��B�oT�n��?���p���0#(��\�~b���M8��]��~{�H�2%8�q�{J�k4o���'ަK�� ""�a�CJn�r�+��O��y�&J���Ȳ�N�'~��%��!گDf��Λ߁�=U}�vveT��--(�ےJ��İ}���)"�"�K�������= qb_40g\����ڻ��ᔷj?L0��r��a}�7�j�.�R���n�H��ч��m7�Ǜ����I��?�:��x�v�c~�ۿU*|5�t��m?8��g)RrUH���=d`�����7����hX㐒�;]ޤd�L�ҡ|�M7��h�i�lt�^R;p��U��RO��O}G���,��X5ȅ�Κ��kT�Ҏ�?�lN��<�&:q�}����!2����";m��:�)�0cE��V�3S1F~�Ď��k�}�\����Fٻ����p�k\�f
�I���m��%��۷�����?xo��Y�\�#�ʢ���ꁡ?j�;{VW�Q�uDDD��!%[˼81���C1��v 8F�t��Q���g�s�~�Ȏ��Yks������m;����J1�l�=���!�܁6*��� ހ��
bӇW�ݹt�޳&�S� w�0 �S��ȧ-��ȡ<\ .;J�h$Eʉ�Bb����+��A%���v>M3[��/���gу��V�\|�]���M����w�̒R2±y�V?����S���o�#""��kRr�����K7S�t���)F�1s�?������Ev�\�`nne���\��c%W�L���^�i7?��eݗ�j*�b�=gL��b�C�`�U;2��QjV���D�ȚW�����bq�������x�ڨ,4pQh`.A�HL��=��?�ث;�/���rH�7S�>�T96�.ڐ��2-�ƽ{���뾫>K�䶌�������e���3�DDD4y�CJn�p��z��x���}�ǃ�D1x�qv�0cE:��?7���#O����������C�Jމͫiq�ai��b���&�T�vB��g����Xj�LT�-�2��ĵ�d�X+�~q	b���X
=�YX�#m{����o"��z�ׂ�/�:�b:j��%K}�o��9_��ĭƎފ�낪����ؤ~�`.VP�����˸�?�A��߱GDDD�5)���宼a�g?:Z"u"wV�8��P(�5Ho;N��ĩ���Xy�\��� ��1�-�]��O��ԁ�vQ ��ϰx\Y+�7��ɗ�:(2��I>������P ( ��M"�K~��b#����?�W��?ڍ6n2`;��j���#O[��=^._zEƋH��\??�������="""�qHɖv�GU��#_Z�����h����z �:)�Zf�,\��}��s�voW�]�����^X�����f�������V����N̊J5y[u���a��ٌ���l�ǹ�g�O��h����-7Y��m.�JM�%w�<SZ��xS[۟�؂�Y�燛߱GDDDc�kJ��:��e��9l�2���>�PE�N�J��k��"sv�޳<��7R2#2���)y�Ό��u6�_UvUMI+~j^�7��7
�2~z����%����dׄ��k����h�|M��ϖ>���y����\a�CU��k^���U�^x���$\��c�|,�߱GDDD��5%�#k�d�̭.򛚚~D䫧��W�^dٮ�57J���{a_[W��릸x~��bRrYmǬ�b�Κ�A���WOꫫ�5�DEɶ��^A���O�}�l��?�5��ʢ���DDD�qH�pPW2g���"Gu��&"���gU\�Ҽ�"s>�d�.��GD=�埧Y|�?�LDDD���٥M�<�*2���&C�`U��Ɲ��F�/]ͪҼ���WN�O�*xc��^��w�����*$D�TDDDt���޿G$�?�z��#�G�{��߭��o5/C���_=��}z�-	���Y�S���=���"""�[�x�d�8u;"�kԼ]���9�e\��֝E��g�7����h�0%O���H��w�P���4ٽ&,�_ BDDD�)9�UW�Լu�/Kh�.��PD�� ""��ŔЪBBJ�=��"#"���dwDd�"�o�b��T������Ehh^�:?h�0�<��� ""�Ɉ)9!��.{�28X�J��"�����g����h�0%"�稘�nE���������9j�6���5�c��.ZO]cgA�V�v��"��5�	DDDt�bJ ȝ��k�kp��|,�`�\�>3��'�$���h�bJ b'ED�����y�a��dw��{DDD4���BO]�V�-����v�����Ξ�U@'""���)Y{H�H~�ǒ5�dX���s�,(�dw�s�_�MDDD��d���e'ED�fw̟�U��=׋�Y2)>�BDDD� �d-�e\̝=kR�""2ҼV�����?i~���h�`J֌�8�Լ�a��\/]�����:L5���="""��dmti�;p�U�v���r�{��NL�w܉��������S��%�����T����q�����="""�3�d�*5"�M��\�#R�?Q�}�������������@lO]�d�|m�dÂ�5��*$�_CMDDD�`J����W-�,����j�i`��'�7�ѭ�)�O���g�L��ܖqQ�ON���5�DDD451%�Cep0r��e�Pos��_�'
���DDDDL��<�O��=u�]�F?h!�c��@�淂����2��	$�DCMX�$��~�T������4ǔ<Q���A�\.{��G����-����H`J��=ׯ,ZX�y%#/��T���o'�����GDDD��)y|X?;*}��5�md>ͫ9㪕k�j[�y���uӈ���Ɣ<>rfݗ{���{��,Z8�>6�p V��/��U!!��DDD8�����&����A���EO.h��׼��C������~!"���d�1%���>�����	�?�D��m>��d�훸SM�g'˟!""�)�)y ��,���I���y�[�C��r*U�[ADDD��������{�����ſ-ZQ0.��M��ya�J�m�M�蹳g�7����( ���*�Be/	=q���۞�<��������f�^��SO?����mm����#�Х�R��WY��*��'�ߓ&""��c�)��w0(\��U���'g�MM}�w���B�����qO�}������]Y��-㢶O^˩�I�"""��Ƙ��+ڑ����梀��c��9f�C0m����W�P���ey3����;��U\��<ҰZ��b��n���o����3�0�̟;��MAcI�+����}.���������G�/��mnGJ���������5ꔜ^����{\4�����k5�p���g��7����(��:%�s�����.�D>�c����w��d1�����N�-_��h�h+��/xr���>j=u�S��I����h$F���X��1��wѤ`�����۞ج�s�YP�?�A�?�ADDD4B�N�[��\*�����Fr�U�a�TY&�H�	]��Y�5�hk��{����w��$2�����R1maxb�Y��5������WlR�7�ɻTnWt�ٝ���Mk���mн_*C>�y��wS�-u�A�+c=N��^�������#��Q��Q�����*i#M�������ͿĄ���hT�?%c�I}-IT���1޵t�{Z�À�a����`+�f����G#��?ҽ�=]���ݣ6�0v̯r(�Q��;⺰��:�-Nd[�݊a�v��
r_��:�A86m�X��&OXUH�y�V�t"""�QKJ��u�����>�F�<�k�=�F�L�,��*�+��ȵt9ߏ�C��5�3w�(Aӑ�� bSі:0q�G��(���n
���	f���V�4 �
���.�1����faw�\g��uF�LgS�78k�j�{�!Kj��u����p �߱GDDD��XR�����L�U���_��I)6�=�.=b@4R�D�s�3�b���|o�o�I�Ģ��=N):�Z�*��aw�b�r�6il���$��v��c*��r~�gs~��WC7�&�t����W˩T~�MFcI�=.w���\k���d4r+ȑh�QC)Y�����,��t1 )^ܞ�u"��teV��rQC)Y:�}q�X��h#%��� /��.V���x8�c(%��t�W���b�c䇢x��Ӣ~����G�h�w�7��5����sJ�mn7,x�Ԃ���&������]*0���O��Kܜh���Nq�Nd_dA�TL�k鮴B�hc0�4ٝb����B������!�h�M�
�9V�N�(�?�Y>�X;�`4p!b#�2��ҭp_W!��a�;���ӑ���Of\]��WK�{{]��T�;����h�KJns�T`�����y��Hɧ/[a{r	?9m|��$�e@1��ÿ��|~�N�1g���\�������51ۅ�����E�[��8%�R'`�����&]�|2��q�N�`,(���d�����W�xl'_S"fI�B�^y������鸇ަ������S���vV������ߞ���ƺ��?�DDDDc6!)�iO\)�"VJqS�y�S�~9�U���@pAY�1=/�<��S�<�K� w������ҡT�����Џ�"�� �G�ty�~�I^���ۧ�HW��|��d���㬶)�).��G�'�����cIɶn�������Kf�`�6щ�yJo�ON�|���܆v矷���{���R�8t_$�ؾ.:K1+?�Y'چ�>�]�_���wRD�c��$��*��E��>v����N�{�W�JE�R'r?z��M	��۾l���_/Y���kMGg=��OJ�����y���GDDD��XRrk�K��:�FV��~�͓z�h�J��s��謲�4v�R��ҥ��E<�=��E�l(��6�*N���
�R�{��;
�_��(�WYg��7}eg�h{�W&޹t���q��j4��:|ެ�o��~{�H�q�ʕ�6e�p��,��d�֭��="""��%%�t�ܕ�Է9�����>�9�՛qS�w�4����mI%�}(��a����cu�6i�|��2R�{��1z�R��:=�4��+�����鸞!�T*�۽¾w?��jL���=Tw���|��J�[[��/�f������G>��㬉N��=׍�V�Zѭa,)��ӥ�M}�����mm��E��q��"�h�ٜ Mxu܌1��x���m�]*w��iޡ43��kT�5��$�J�o1���}qv�w"�J=�վ�&����z���"��QH��o-Лs:o���3�F>�O�Á����.�$UW��h�@����dk�K��Dq�D�����4/8F�Cя;O��V4"�Bq��y�s�X��v��DL�	?V�� ����ìr�bn�PJƔ�m��l��D��L�ŞͳI��F�t+�}o�4�,.J�K҅�=kR�T�����A�ǡ__<-��ǟ��[�u����a�)]�,�c����ncI�Mv�
ȭ�m�͐�<�L/�G��|/Y�_,s���6>�:.!�r&׆����9c2�:�7�b�������=V�O�픀�0}Ap�bv�M3�LD��RQ�?�Fe)n����㗬�!f���K�b�\�+���pܻw&�v�?�Αw�-l_��a_�	z�:���ǒ5�������XRrc��]B��x�?��Ud@t"�ANEک96DC����d�XS�┦_(u�E�̰�C��,���ܤ{c�^��M=#`d�	�hW�Ȕ�����+&bSi��y'6K�!z��ua|�93vD.w �`�v� �^܇�R���,�vq�8%�;K}��y1GU����䞺��9vi�(����������<��ND��,�t����hx�Y��0�;5�5�*uD�1ᔘ��ᣣ%�\ч��?b��FL��8�䪨��7*��^�q����xl��<ma���Tb�ǃo~�{\ׅ��w���tT�q�Ͳ��#b���f�Rrep0�c����n=cIɖv�7Q���f�� w_�8
�F5e�!���$�B���V�8������AU�c���H�����DDDtKuJ��0�duַ���~��|�&NDJFD.~f	c����nI�N�sVǝ�l�</NA���%�l�k�1��y��{�G��s�0�̟��ܮ�LDDD4F��W���x�Pgs�?�}S��<��G�W/	=>^MO]cW������na�N��ϖ>�����"�1~z2���j*�ǼB��[.����sݰ�q����F���5�S�m�V�G��ݦ|˘������¾���qyb�BB*��5p����&�XRrYmǬ�b�ΚM�����_.�e���>��ѳ9�qy\�J�Sc����nycI�pPW2g���"Gu��&Hť���2�ԏy���~D��CY��t�s��<�?�FDDDS�S2d�6=���Ȍc�5�U�.G��W��ʎ��0����R����{���׻�=u����;����h�{JG��#��{=�����h\���O���3}}l��r�Eْpy�>���s����-���+����i" �?��nG��H*֮�z����&Sr`��Z��h^��߱GDDDSSr`	�wm�[N���5j^	�?1%�����z�V����MALɁa�).>p"��x4JҼ""""�cJ�ǒ�,Z�yr=u���""""bJ�^[���ٳ��+�4�eD&""���)Yc���]�Fм���=�y%DDDDZaJ֒�T�<P�"�y�Ve�� """�S�f�_����4�D��sݸje��!�V����$
���ϕ��U!!��ADDD�9�d�Ys�jJ�=8�����HCL�~R��@�<�O�����$ס�m>��yDDDD�)�:r���|��?�_�;z���C��Ο�`gA���d�ڰ)r��G��,ּ��������ADDD8����ʢ�"%C�C?����|�?jADDD�������'"r��?.��s��� �Ɉ���,�o�)0%O�kv��޻/��޲��̟{e�Bd�@�Hꨇ߱GDDD�n<SrAe[��%�'�Y}��I�߿x[��b�{�ws���y=RU3}�=��ǳx�:���]j��%"""��I�ݽ�Aẟ��}�>9�lj�����V_E���6 � ^G��?[����l��?�DDDD�4)9������x�o.�L!�U�����}/Ĝ�1k�����)��w��֡y���Vu�,�=7F>������n͟W""""��5%�تۯ3��hR�e��y����NL/�>�z���+������zb&�κւy��
��6}E�籺�Y""""?�)%�s�����.
|_;nt5u7��
�u�A�g5d������������N�-_��(�|�f�n_V�|���U5d��������|�∆�AG��\���W�<��}��un{b��,���������&B�u��>�>&�hW`�vb�Q��fA��;�c�e�}�܄���}$#�7��є��h���uaJ&""�)�ה����۹���dp?�Ǐt8�m���񮥻��U�L>:1ӬR�/�'=�2����+6��7�f���E���F���G�0Q�W~�c��p\Ȱ�K���y�����(�o$[�[�i��㩶���y�:Z�G^�
�d"""�"&*%�艤�ا�GIJ�0�Η��{����u}O!��]DlEЌL)�م5�3����(�P9��]DcX���[�*���2�R�{�H�`S�щS�
����D����F��ju��Ձ�cJ&""���ה���R��g�߼���DvܓjT���a�04*�w�(�Yevm����)&���)�&�~�D�]���o��iñ2�͵bQ!fݱ8��˩^��o���1~��)3�b��S!R2�V��ߏ���N	&ƞ3I��/Y0 ��Zk���NF�LgS�78�qS2M��d{�KEs���ܧ�|t]bt�Q}�\+B�hg���*����ǲh#%+G?�"�)�����}@�0aM�`���s�p<˂}�Y_ܞ.��k�R*ec�N}��ջ21We"�}r}�|VH7���Dq+D�شm��)���p6G�;��qS2M����h!�F��Ǥ�Z���C�L�Wk���p�ܧ��f��V:а%f�Ϣ�Y�	��Qr��!)�"�/�����q(b7K�������(X@����R�bFz����Aq�%���i��%�OA���y�*����
����ϛ�Z����E���Aop��,�d"""�"|M��_�T����9)��Q:<�������B��D�[�����p
��%�9V�� L|~�NFJ.��m��1r��ɚ�&N�)<�>	�Mc��̠�������2h�1 �JmX�;L���bS��������(?���Ĝ

��B0�iԗ������o:=���~��8�)�����_Sr�å������̷����.Z��7��#L.���^�'1�P��k��i�d��?AJެm��aҩ�J��6��t6�Y>�c�(�\���Z�����L��"�ԉuT����r���e ;J��>`k�����V��o��􊥾������{��<��z�ŔLDDDS���d	rқ{?�&���O�8r$��zJ��;gM�8��+�#���lU��"P�!�!"��(m7���
q����v�.�]�
�8��.����:o�I�� ��^a�8<���~��hoN4x������8�=���H�Y�d"""��|Mɶn�7�꾻��v￙�OU&
���������nB�۬SPl��E���7?��qrI�u��{?��� ����TLy��o&�'�z���݉Ɵ����A�H0[(`�މ����E*�q�XgfPLf�]�.a�7g]t�-�/���@66U��)�wۗ��z�ŔLDDDS��)����M�PJv�G��}ʨ2Qv������)� :w�d����B>���+;3����¶t�,�@?�;��զ-GlU�DU��\l*��ޡ<,{Rou�,�0��D�\��"����p��8����_�E�E�E��Ql�R���Ql����Mh��U|�R�������Ne��-���z��-dJp��,�d"""�"|M�-].o
�n�d��y�&�:iT�(��%2yW��DJ����B�K�>L0 Vַ9��4�7�Ж�A��R��Ai�Ͼ�Hkb"� 2+�����Xg���ۘ��?l͘���Q�����a���܄JP�8�X> =�r{Q�8�L/K���{�'!.K�8��w��[��Q3OG�H���#��qS2M����N�7���1N�?˴H�"%�LR�����6�䝘(�`ql!�%��'��r��l|fc��L4�!��ٜ�;�f�`�^�f�S3V���R�ڤ�p�#��z����Kwu��;���D�)�}^]��ō���QH��o-
���)8��to������h��5%[;]����Z�0��!�#��<iT������i�Y�� �P\;��!�ަ�胶�K�����/��l��)���i`k�)���_�U/P�ë��#Q��,��]��<1��щEP<6�_�p�Ȏ)���˩�:��z��#.d�R!>���æ�|����Uf1%��kJn����X�s�.����Tѣ�^dǘ�L��K���[هΫ��H��aȈ����M3c��J�Sh �b���BPx�x�����}z� 8I�������+�ygHl�:�k�6kmT֢)�,\/�Kgq���}�6��L�����]I�X�2P-n���ƽ{���뾫>�)�����_Src�˛���&��.R�	��)Ɔ�7���~����	;b@PFg�9�Xj���,+�-/�PL�b؊�t�F,R��T)�Ԓ�T��ܑ��[��nHy<8	�>w���������4�]�.G����E���j�ð;�aNE�ǚ�;R��~p��i��ʘ��pEJ�>*L�DDD4E���:\*���H�;N=��ϰT�8��gL�^��^����}8Dfu_a�/� ��P�BHͱ�� ���39ˊ�G>�����3K=hc/����W��+n�a��yR�GGK�cpQ"�"+���㲸Q��mؕ���>`"���G�)�����_S���5Z�0V�vֹB{R�U:�J5)�αae���@%��`l�m��>���վ��R��Dy#�3#����?k���
?0��`̘����h��)%O[n�:��\��?�R��&�ȔLDDDS�O)y��S�m���)ȔVh.i�k���M�L��,����%"""��R���l.�	�ܟ�3�������KB�k����O)y���g?���\�7�쪜�g�2���u��[.k����O)Ys8%�fnu����W_���(��֥u�������_�G�����|M�e��^�568kZ\4�
~��d�n��[��ϧ�>z6Ǭ��JDDD���d8�+���pz����E�ʆM��_��}K���Cei����8�d�.mz`��U��.6j��]4�LU�e�2*˻��ci��d7����}/���DDD4ՌOJG��#��{=����=�����G_?����Fn���斄��,2MA㖒i�\�;
��m>��y%DDDDSSr�s�j�j^є�j���vDj^�TÔ�ZN�̟{��м"""���)9p��n�,(Ҽ"""�)�)9]�;J�=�w��������k��4/����h�bJ8�E�U+�{�k^	єŔXZN��O#i�)9�t�Ξ�UjԼ"""�)�)9�T�]kӥi^1%����u;"�G-����Sr@�	+]���e������R#�c����(�0%k���������(�0%k����`�ܖS��WBDDDDrL�Z2�Zi޺U�2����H�)Y3����v�� """"wL��h>����#"""
XL��*5�;�����S��]�;�����(�1%�U���e���Լ""""R���W5aa�AҼ""""Rǔ�?�쎶����="""��ǔ<��6�+^���^�΂��92"M
L���W��
������`�\�.M󒈈��h$��'�Օ+��!���7mּ""""!��	t��E"%Cά�m�м$""""	��	����""_y��k��3��\ͫ""""�a1%O���?,�7�|ş��<X�YP�yIDDDD4㖒*�Be/	=q���۞�L�������ϟ~dſ,�@�bF� ^��C��K��?�DDDD�����;��ɪ��铳̦�����h��+�������=���[��)������+ڑ�����[Oj��b��5R�����ɧ���;�U\��<���i�«����[󇕈���o|J�+����}.���Z{=A󇕈���oƞ���zb�����J4^�����c�)�͘����\w�T�_W~V�畈���?ƞ��V�I���~M�������+��=%߱8��c���)�'6k�����S22S�5�D��غ��c���q�w�M'Ԙ�����?2%���SJ��sy���|�H��:�~����1z�(`���K��T�`��l����4�U_Y��y���W9��x9�ZoS��#SJFX���%��7k��V{K�S2M��E�k�.�tς[���2�!b��=�[�s����+�,�bkt��+c���h��^niX*.�cp�}X�;S1^�v�fyL��k�)��V(���Ձ�cJ&""�)Χ����R�~\�o�MQt"�I5�O� C���pǉџUfG�h�_jK�t�ME���gs���l��;bi"T6�/��)�}p�D�v�BF#1^1]1ŋ�-�"��s&y��t9��3����z�R͟W""""��)%�{\*�;���>E���S����ZY'�Y���J�hc"��,�H��ϲH�G����\l7���H��u��.o�+���o�I��webe�[��VT4;�����(�t'��]���+����;z\����jT��kE��_ܞn�tb"R��Ā+�1p��.?̭t$gYD���I�W�b�Q-��୒ԡ�������a�Cy�����#p�i[}���~c;��z�R͟W""""��)%��R��cu�|�(��,��
m8����[tH~�z8뀱a =8%#��)� �`L�H�Aq�D��dwJ�`S�5%I-O��H�%X��,T��U�K�;��˩p\(�K�o�:���ӑ��d���YL�DDD4u����.���?Nk��/;o��s���f�u{��	ӟ�F�mt��'��b���e CM�����f�hcm�W��щ5Q���V�k�Y���)��\�*�/�U��*�+�b�T��@a�[K0��sG8Q~+�������J�F��M�)op��,�d"""�:�9%K�ې�<fA)��/�����M@t��r��*�촅�ۓK�+�V*v�'i	�UIɛ���"�m�G�*nTM� N���5Jp����L�Nb$������ӿq�{~/ّ��L�DDD4����m�.o�}w?��3%�2�L�\�+��Yl������s�ub ���[�5����K��׿w(O1W�~�b��ű �U�E��A4ڝ*��͹}qn˺�,�sS�W�>1%��o����YoW���JDDD�>���n�7�C)ٽ�q�)��Di���fK�sFP"���=��E�c�Y'�V���7�2�������cAŔ��M��\��e��H�b�a/^ٙ�jtV�up$��с�,�ǥ���q����E�_�\��~{�H�2%8��J5^�����ç������fJv��j⮓F��1�W"3�1�O��D�d�����}qS4�ۜ���W�Y���_�55J=&���*�_��^�����S�u��b��E%����q��W$3��q��?��R���c~�ۿU*|5�t��m?8��ޮT�畈���?|J�͝.o�M7c�hJ3K�"%�LR����/ۤ�wb�ԃű�b�D4���#t"j:Ec۱�+bVEfz�Q���~�b�{%�U �z<�
�]�e^*w��e��Υ��ْ��zfc�8������}q��`�0�0�����A��q~��7]�J5^�����ç�l�ty�7��kmN���y6�at�I��D�h\���__;�m�:?�7`M��X��Yŵ���J���m��`��b�|;��e��]$Xu���Td\�.�o�T'~~�fF���=���47����S��
�w��6��O�߭~��?�DDDD��SJn����X�s��Ia�y?�hd�Qebz�c2-�if�p�<�Ns�s�&�|2bne�h�l���gmT֪�*�{���/Y���/S�sƄ��p����^�
�8`ц\�h���N,�['���
F���A������T�|���޽���u��J5^�����ç�����&!Â7�(��"%�0z�bl|c�~�'Yh��wb��Î��nҡ'5ǖS�����a�H��,��.��n��,�d�����I�XJ��tl�r���)Y���#�*Ƨ�'�Юiqb��sf�,\,:Q'\(u��}qg�/��&KcP���T�t�K�+�ӽ��d"""�:|J�.Hi��E'��F���3,�-NE�؛Xn^��)�ȇ�O<xΌ0�b����OβʋA���Uq�o#�/S���NG��"E�Ⱦ��*����5���m_����d"""�:|Jɖv�h!"V�jJU�3)�z:�&�D���9��U`�2ˠb_T;�D�,�9�����?wdJ&""��c�)y��p��Y�梩�)���������9��N]�i���?�L��,���y%"""򏱧��;366��\49_�$����+��=%�?[�쇺Z������$\��y%"""򏱧dxd��l���E��Һ��^���կ��JDDD�>��ڎY/��5-.�Uյ�󩷏��1k����O)�J�9�^�nqѭ���9�P��O*�?���!��違WEf��d��jv�dWZ�_)�Mo�p���.2MA㐒��������^��cq�mOl���#^�-	��Yd"""���'%�J�������������������������������������������������������������������������������������������������������������������������? �wd�"e    IEND�B`�PK��2�S�  I�  PK  ��VO               META-INF/manifest.xml�R�<?xml version="1.0" encoding="UTF-8" standalone="no"?><manifest xmlns="urn:xmind:xmap:xmlns:manifest:1.0"><file-entry full-path="content.xml" media-type="text/xml"/><file-entry full-path="META-INF/" media-type=""/><file-entry full-path="META-INF/manifest.xml" media-type="text/xml"/><file-entry full-path="meta.xml" media-type="text/xml"/><file-entry full-path="Revisions/" media-type=""/><file-entry full-path="Revisions/4c8cdrtv5uli10r8nr70grk327/" media-type=""/><file-entry full-path="Revisions/4c8cdrtv5uli10r8nr70grk327/rev-1-1571736424210.xml" media-type=""/><file-entry full-path="Revisions/4c8cdrtv5uli10r8nr70grk327/rev-2-1571736578774.xml" media-type=""/><file-entry full-path="Revisions/4c8cdrtv5uli10r8nr70grk327/revisions.xml" media-type=""/><file-entry full-path="styles.xml" media-type=""/><file-entry full-path="Thumbnails/" media-type=""/><file-entry full-path="Thumbnails/thumbnail.png" media-type="image/png"/></manifest>PK3�K�  �  PK   ��VOiwQ,  '                   meta.xmlPK   ��VO<ӵ,
C  C               b  content.xmlPK   ��VO�0��    
             �D  styles.xmlPK   ��VO��Q%     2             �P  Revisions/4c8cdrtv5uli10r8nr70grk327/revisions.xmlPK   ��VOuWTq�B  �B  <             {S  Revisions/4c8cdrtv5uli10r8nr70grk327/rev-1-1571736424210.xmlPK   ��VO�&�7C  C  <             ٖ  Revisions/4c8cdrtv5uli10r8nr70grk327/rev-2-1571736578774.xmlPK   ��VO��2�S�  I�               a�  Thumbnails/thumbnail.pngPK   ��VO3�K�  �               �� META-INF/manifest.xmlPK      d  ��   