# utl-universal-language-translator-using-python-package-googletrans
Universal language translator using python package googletran
    Universal language translator using python package googletran

    github
    https://tinyurl.com/v45nczy
    https://github.com/rogerjdeangelis/utl-universal-language-translator-using-python-package-googletrans

    also see
    github
    https://tinyurl.com/ycgk5rmd
    https://github.com/rogerjdeangelis/utl_npl_star_trek_universal_language_translator_sort_of


    *_                   _
    (_)_ __  _ __  _   _| |_
    | | '_ \| '_ \| | | | __|
    | | | | | |_) | |_| | |_
    |_|_| |_| .__/ \__,_|\__|
            |_|
    ;

    %let text='bonjour madame';


    *            _               _
      ___  _   _| |_ _ __  _   _| |_
     / _ \| | | | __| '_ \| | | | __|
    | (_) | |_| | |_| |_) | |_| | |_
     \___/ \__,_|\__| .__/ \__,_|\__|
                    |_|
    ;

    %put &=english;

    ENGLISH=Hello Miss

    *
     _ __  _ __ ___   ___ ___  ___ ___
    | '_ \| '__/ _ \ / __/ _ \/ __/ __|
    | |_) | | | (_) | (_|  __/\__ \__ \
    | .__/|_|  \___/ \___\___||___/___/
    |_|
    ;
    %utl_submit_py64("
    import pyperclip;
    from googletrans import Translator;
    translator = Translator();
    text = translator.translate('bonjour madame', src='fr', dest='en');
    print(text.text);
    pyperclip.copy(text.text);
    ",return=english);

    %put &=english;

    Hello Miss

    *_
    | | ___   __ _
    | |/ _ \ / _` |
    | | (_) | (_| |
    |_|\___/ \__, |
             |___/
    ;


    MLOGIC(UTL_SUBMIT_PY64):  Beginning execution.
    MLOGIC(UTL_SUBMIT_PY64):  This macro was compiled from the autocall file c:\oto\utl_submit_py64.sas
    3600   import pyperclip;
    3601   from googletrans import Translator;
    3602   translator = Translator();
    3603   text = translator.translate('bonjour madame', src='fr', dest='en');
    3604   print(text.text);
    3605   pyperclip.copy(text.text);
    3606   ",return=english);
    MLOGIC(UTL_SUBMIT_PY64):  Parameter PGM has value "import pyperclip;from googletrans import Translator;translator = Translator();text = translator.translate('bonjo
          madame', src='fr', dest='en');print(text.text);pyperclip.copy(text.text);"
    MLOGIC(UTL_SUBMIT_PY64):  Parameter RETURN has value english
    MPRINT(UTL_SUBMIT_PY64):   * write the program to a temporary file;
    MPRINT(UTL_SUBMIT_PY64):   filename py_pgm "d:\wrk\_TD5684_E6420_/py_pgm.py" lrecl=32766 recfm=v;
    MPRINT(UTL_SUBMIT_PY64):   data _null_;
    MPRINT(UTL_SUBMIT_PY64):   length pgm $32755 cmd $1024;
    MPRINT(UTL_SUBMIT_PY64):   file py_pgm ;
    SYMBOLGEN:  Macro variable PGM resolves to "import pyperclip;from googletrans import Translator;translator = Translator();text = translator.translate('bonjour mada
                src='fr', dest='en');print(text.text);pyperclip.copy(text.text);"
    MPRINT(UTL_SUBMIT_PY64):   pgm="import pyperclip;from googletrans import Translator;translator = Translator();text = translator.translate('bonjour madame', src='fr
    dest='en');print(text.text);pyperclip.copy(text.text);";
    MPRINT(UTL_SUBMIT_PY64):   semi=countc(pgm,';');
    MPRINT(UTL_SUBMIT_PY64):   do idx=1 to semi;
    MPRINT(UTL_SUBMIT_PY64):   cmd=cats(scan(pgm,idx,';'));
    MPRINT(UTL_SUBMIT_PY64):   if cmd=:'. ' then cmd=trim(substr(cmd,2));
    MPRINT(UTL_SUBMIT_PY64):   put cmd $char384.;
    MPRINT(UTL_SUBMIT_PY64):   putlog cmd $char384.;
    MPRINT(UTL_SUBMIT_PY64):   end;
    MPRINT(UTL_SUBMIT_PY64):   run;

    NOTE: The file PY_PGM is:
          Filename=d:\wrk\_TD5684_E6420_\py_pgm.py,
          RECFM=V,LRECL=32766,File Size (bytes)=0,
          Last Modified=15Apr2020:14:47:52,
          Create Time=15Apr2020:13:36:11

    import pyperclip


    from googletrans import Translator


    translator = Translator()


    text = translator.translate('bonjour madame', src='fr', dest='en')


    print(text.text)


    pyperclip.copy(text.text)
    NOTE: 6 records were written to the file PY_PGM.
          The minimum record length was 384.
          The maximum record length was 384.
    NOTE: DATA statement used (Total process time):
          real time           0.01 seconds
          user cpu time       0.03 seconds
          system cpu time     0.00 seconds
          memory              446.03k
          OS Memory           22276.00k
          Timestamp           04/15/2020 02:47:52 PM
          Step Count                        743  Switch Count  0


    MPRINT(UTL_SUBMIT_PY64):  quit;
    MLOGIC(UTL_SUBMIT_PY64):  %LET (variable name is _LOC)
    MLOGIC(UTL_SUBMIT_PY64):  %PUT &_loc
    SYMBOLGEN:  Macro variable _LOC resolves to d:\wrk\_TD5684_E6420_\py_pgm.py
    d:\wrk\_TD5684_E6420_\py_pgm.py
    SYMBOLGEN:  Macro variable _LOC resolves to d:\wrk\_TD5684_E6420_\py_pgm.py
    MPRINT(UTL_SUBMIT_PY64):   filename rut pipe "C:\Python27\python.exe d:\wrk\_TD5684_E6420_\py_pgm.py";
    MPRINT(UTL_SUBMIT_PY64):   data _null_;
    MPRINT(UTL_SUBMIT_PY64):   file print;
    MPRINT(UTL_SUBMIT_PY64):   infile rut;
    MPRINT(UTL_SUBMIT_PY64):   input;
    MPRINT(UTL_SUBMIT_PY64):   put _infile_;
    MPRINT(UTL_SUBMIT_PY64):   run;

    NOTE: The infile RUT is:
          Unnamed Pipe Access Device,
          PROCESS=C:\Python27\python.exe d:\wrk\_TD5684_E6420_\py_pgm.py,
          RECFM=V,LRECL=384

    NOTE: 1 lines were written to file PRINT.
    NOTE: 1 record was read from the infile RUT.
          The minimum record length was 10.
          The maximum record length was 10.
    NOTE: DATA statement used (Total process time):
          real time           1.49 seconds
          user cpu time       0.01 seconds
          system cpu time     0.03 seconds
          memory              315.40k
          OS Memory           22276.00k
          Timestamp           04/15/2020 02:47:54 PM
          Step Count                        744  Switch Count  0


    MPRINT(UTL_SUBMIT_PY64):   filename rut clear;
    NOTE: Fileref RUT has been deassigned.
    MPRINT(UTL_SUBMIT_PY64):   filename py_pgm clear;
    NOTE: Fileref PY_PGM has been deassigned.
    MPRINT(UTL_SUBMIT_PY64):   * use the clipboard to create macro variable;
    SYMBOLGEN:  Macro variable RETURN resolves to english
    MLOGIC(UTL_SUBMIT_PY64):  %IF condition "&return" ^= "" is TRUE
    MPRINT(UTL_SUBMIT_PY64):   filename clp clipbrd ;
    MPRINT(UTL_SUBMIT_PY64):   data _null_;
    MPRINT(UTL_SUBMIT_PY64):   length txt $200;
    MPRINT(UTL_SUBMIT_PY64):   infile clp;
    MPRINT(UTL_SUBMIT_PY64):   input;
    MPRINT(UTL_SUBMIT_PY64):   putlog "*******  " _infile_;
    SYMBOLGEN:  Macro variable RETURN resolves to english
    MPRINT(UTL_SUBMIT_PY64):   call symputx("english",_infile_,"G");
    MPRINT(UTL_SUBMIT_PY64):   run;

    NOTE: Variable TXT is uninitialized.
    NOTE: The infile CLP is:
          (no system-specific pathname available),
          (no system-specific file attributes available)

    *******  Hello Miss
    NOTE: 1 record was read from the infile CLP.
          The minimum record length was 10.
          The maximum record length was 10.
    NOTE: DATA statement used (Total process time):
          real time           0.02 seconds
          user cpu time       0.00 seconds
          system cpu time     0.03 seconds
          memory              331.65k
          OS Memory           22276.00k
          Timestamp           04/15/2020 02:47:54 PM
          Step Count                        745  Switch Count  0


    MPRINT(UTL_SUBMIT_PY64):  quit;
    MLOGIC(UTL_SUBMIT_PY64):  Ending execution.


