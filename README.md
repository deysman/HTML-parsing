HTML-parsing
============
A small HTML parser implemented in Racket that takes a string HTML representation and returns a list of individual elements within the scope of the root tag.

##Example
Input:
'<html attr1="hi" attr2="bye"><body><h1>Heading!</h1><div><p>Paragraph.</p><h2>Subheading.</h2><p>Paragraph.</p></div></body></html>'

Output:
'(("html"
   (("attr1" "hi") ("attr2" "bye"))
   ("body"
    ()
    ("h1" () "Heading!")
    ("div" () ("p" () "Paragraph.") ("h2" () "Subheading.") ("p" () "Paragraph."))))
  "")
