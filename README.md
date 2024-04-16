# sentence-analysis
ALGORITHM algorithm_name
VAR
    c : CHAR
    nbrChar, nbrV, nbrW : INTEGER
BEGIN
    nbrChar := 0
    nbrV := 0
    nbrW := 0
    REPEAT
        Read(c)
        nbrChar := nbrChar+1
        IF (c = 'a' OR c = 'e' OR c='o' OR c = 'u' OR c = 'i' OR c = 'y') THEN
            nbrV := nbrV+1
        END_IF
        IF (c = ' ' OR c = '.') THEN
           nbrW := nbrW+1
        END_IF
    UNTIL (c='.')
    Write("number of characters = ", nbrChar)
    Write("number of vowels = ", nbrV)
    Write("number of words = ", nbrw)
END
