# sOption-
Func _WD_FrameEnter($sSession, $sIndexOrID) .....     ;*** Encapsulate the value if it's an integer, assuming that it's supposed to be an Index, not ID attrib value.     If IsInt($sIndexOrID) Or IsKeyword($sIndexOrID) = $KEYWORD_NULL Then         $sOption = '{"id":' &amp; $sIndexOrID &amp; '}'     Else         $sOption = '{"id":{"' &amp; $_WD_ELEMENT_ID &amp; '":"' &amp; $sIndexOrID &amp; '"}}'     EndIf .....
