# StringInStr
 Func _GetDelim($sTest)     If Not IsString($sTest) Then Return SetError(1, 0, "") ; Invalid Input String.      Local $aAscII[31], $sDelim ; Using Control Characters only.     ; First try one character     For $i = 1 To 31         $sDelim = Chr($i)         If Not StringInStr($sTest, $sDelim, 1) Then             Return $sDelim         Else             $a
