## ራስዎን ይፈትኑ

<head>
  <meta http-equiv="X-UA-Compatible" content="IE=edge" />
  
  <meta http-equiv="content-type" content="text/html; charset=utf-8" />
  
  <meta name="viewport" content="initial-scale=1.0" />
  
  <title>
    ፈተናዎች
  </title>
  
  <!-- jquery for maximum compatibility -->
  
  <link type="text/css" rel="stylesheet" href="https://stackpath.bootstrapcdn.com/twitter-bootstrap/2.2.1/css/bootstrap-combined.min.css" />
  
  <!--<script src="http://ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js"></script>--> <script src="https://code.jquery.com/jquery-1.11.1.min.js" integrity="sha256-VAvG3sHdS5LqTT+5A/aeq/bZGa/Uj04xKxY8KM/w9EE=" crossorigin="anonymous"></script>
 <script src="https://stackpath.bootstrapcdn.com/bootstrap/3.3.5/js/bootstrap.min.js"></script>
 <script></p>

<pre><code>var quiztitle // = "የቦቢ የናሙና መጠየቂያ";

/ **
* እዚህ ስለሚነሱት ጥያቄዎች መረጃ ያዘጋጁ. ሕብረቁምፊ ማመሳሰል እንደመሆኑ መጠን ትክክለኛው የአጻጻፍ ክር
* ትክክለኛውን ምርጫ በትክክል ማሟላት አለበት. (ለጉዳዩ ትኩረት)
*
* /
</code></pre>

<p>/ **
* የጥያቄዎቹን ተመጣጣኝነት (Randomization) እንፍጠር!
* /</p>

<p>ተግባር ሽንት (ድርድር) {
  var currentIndex = array.length, temporal value, randomIndex;</p>

<p>// ለመቅየል አካላት እየቀጠሉ እያሉ ...
  (በ 0! == currentIndex) {</p>

<pre><code>// ቀሪውን ክፍል ይምረጡ ...
randomIndex = Math.floor (Math.random () * currentIndex);
currentIndex - = 1;

/ እና ከአሁኑ አባል ጋር ይቀይሩት.
ጊዜያዊ ቫልሉ = ድርድር[currentIndex];
ድርድር[currentIndex] = ድርድር[randomIndex];
ስብስብ[randomIndex] = ጊዜያዊ ቫልጌ;
</code></pre>

<p>}</p>

<p>????? ???
}</p>

<p>(! (Array.prototype ውስጥ "መንጠቁ")) {ከሆነ
  Object.defineProperty (Array.prototype, "መንጠቁ» {
    ሐሰት: enumerable
    ተግባር () {: እሴት
      = ይህ var o, i, ln. ርዝመት
      ; (ln-) {
        i = Math.random () * (ln + 1) | 0;
        o =[ln]
        ይህ[ln] = ይህ[i]
        ይህ[i] = o

      ይህ,
    }
  });
}</p>

<pre><code>var quiz = [
    {
        "ጥያቄ": "ስክሪፕቶች ትክክለኛ ቦታው ነው የሚሉት የትኛው ነው?",
        "image": "images / montage-1..png",
        "ምርጫዎች": [
                                "A",
                                "B",
                                "C",
                                "D"
                            ],
        "ትክክል": "A",
        "ማብራርያ": "ከ 0 በላይ ያለው X ቦታ ከማያ ገጹ በስተቀኝ ይገኛል" ,
    },
    {
        "ጥያቄ": - "ስክሪፕቶቹን በ 90 ዲግሪ አቅጣጫ ወደ ጥቁር አረንጓዴ ሲነካ ምልክት ያለው የትኛው ነው?",
        "image": "images / montage-2.png" ,
        "ምርጫዎች": [
                                "A",
                                "B",
                                "C",
                                "D"
                            ],
        "ትክክል": "B",
        "ማብራርያ": "sprite ማንኛውም ቀለም ከነካ ከ
        ሰከንዶች በሺን አንፃር በ 90 ዲግሪ ጠቋሚዎች,
    },
    "ጥያቄ": "ከየትኛው ስክሪፕት ውስጥ በ 1 ኛ ክፍለ ጊዜ ውስጥ ከ 10 ሰከንዶች ውስጥ የሚቆጠር ነው?",
        "image": "images / montage-3 .png ",
        " ምርጫዎች ": [
                                " A ",
                                " B ",
                                " C ",
                                " D "
                            ],
        " ትክክል ":" B ",
        " ትርጓሜ ":" ተለዋዋጭ 10 ላይ ይጀምሩ እና በ -0.1 በየ 0.1 ሰከንድ ",
    },

] ይቀይሩ.
</code></pre>

<p>// ይህን ለ IE የአስተዲክሽት ስህተት በ <>: ECMA ስክሪፕት 6 በ IE 11 አይደገፍም (
0_quiz.forEach (function (q) {return q.choices.scramble ()});</p>

<p>// ይህንን ለ ECMA ስክሪፕት ለመጠቀም 6
// quest. ForEach (q => q.choices.scramble ());
//console.log (ጥያቄ[0]ቅጅዎች);</p>

<p>ጥያቄ (quiz = shuffle (quiz));</p>

<pre><code>/ ******* ከዚህ መስመር በታች ማርትዕ አያስፈልግዎም ********* /
var currentquestion = 0, score = 0, submt = true, selected;

jQuery (ሰነድ). (እንደ (ባለ ተግባር ($)

    / **
     * ኤች ቲ ኤም ኢንኮዲንግ ተግባር ለተራታች መለያዎች እና አይነታ ባህሪያት በመደበኝነት ባህሪያት ውስጥ የሚታዩ የተበላሸ
     * ውሂብ ይከላከላል.
     * /
    ተግባር htmlEncode (value) {
      return $ (document.createElement ('div')) text (value) .html ();
    *

    / **
     * ይህ ለእያንዳንዱ ጥያቄ የግለሰብ ምርጫዎችን ኡው # ዱን #
     *
     * @param {choices} አደራደር ውስጥ ይጨምረዋል. ከእያንዳንዱ ጥያቄ
     * /
    ተግባራት (ምርጫዎች) {
        if ( አይነት ምርጫዎች ምርጫ! == "ያልተወሰነ" &amp;&amp; $ .type (ምርጫዎች) == "ድርድር") {
            $ ('# ምርጫዎች-block'). ባዶ ();
            ለ (var i = 0; i&lt;choices.length; i++){
            $(document.createElement('li')).addClass('choice choice-box btn').attr('data-index', i).text(choices[i]).appendTo('#choice-block');
            }
        }
    }

    /**
     * Resets all of the fields to prepare for next question
     */
    function nextQuestion(){
        submt = true;
        $('#explanation').empty();
        $('#question').text(quiz[currentquestion]['question']);
        $('#pager').text('Question ' + Number(currentquestion + 1) + ' of ' + quiz.length);
        if(quiz[currentquestion].hasOwnProperty('image') &amp;&amp; quiz[currentquestion]['image'] != ""){
            if($('#question-image').length == 0){
                $(document.createElement('img')).addClass('question-image').attr('id', 'question-image').attr('src', quiz[currentquestion]['image']).attr('alt', htmlEncode(quiz[currentquestion]['question'])).insertAfter('#question');
            } else {
                $('#question-image').attr('src', quiz[currentquestion]['image']).attr('alt', htmlEncode(quiz[currentquestion]['question']));
            }
        } else {
            $('#question-image').remove();
        }
        addChoices(quiz[currentquestion]['choices']);
        setupButtons();

        jQuery(document).ready(function($){
            $("#question").html(function(){
                var text= $(this).text().trim().split(" ");
                var first = text.shift();
                return (text.length &gt; 0? "&lt;span class='number'&gt;" + መጀመሪያ + "&lt;/span&gt; ": መጀመሪያ) + ጽሑፍ.join ("");
            });

            $ ( 'p.pager') እያንዳንዱን (ተግባር () {.
                var ጽሑፍ = $(this).text () መከፋፈል ( '.');
                (text.length ከሆነ &lt; 2)
                    ; መመለስ

                ጽሑፍ[1] = '&lt;span class="qnumber"&gt;'+ text[1]+'&lt;/span&gt;',
                $(this).html (
                    text.join (' ')
                ),
            });

        });

    *

    / **
     * ከተመረጠ በኋላ, ትክክለኛውን መልስ
     *
     * @param {choice} ቁጥር ይመርጣል. የተመረጠውን ዜሮ-ተኮር አመልካች
     * /
    የሂደት አሰራር (ምርጫ) {
        if (ጥያቄ[currentquestion]['ምርጫዎች'][choice] == ጥያቄ ቁጥር[currentquestion]['ትክክለኛ']) {
            $ ('ምርጫ') eq (ምርጫ) .addClass ('btn-success'). css ({'font-weight':'bold', 'border-color':'#51a351', 'color':'#fff'});
            $ ( '# ማብራሪያ') HTML ( '.&lt;span class="correct"&gt;ትክክል!&lt;/span&gt; ' + htmlEncode (የፈተና ጥያቄ[currentquestion][ 'ማብራሪያ']));
            ነጥብ ++;
        } ሌላ {
            $ ('ምርጫ') eq (ምርጫ) .addClass ('btn-danger'). Css ({'font-weight':'bold', 'border-color':'#f93939', 'color':'#fff'});
            $ ( '# ማብራሪያ') HTML ( '.&lt;span class="incorrect"&gt;ያልሆነ!&lt;/span&gt; ' + htmlEncode (የፈተና ጥያቄ[currentquestion][ 'ማብራሪያ']));
        }
        የወቅቱ ጥያቄ ++;

        if (currentquestion == quiz.length) {
            $ ('# submitbutton') .htm ('btn-success'). AddClass ('btn-info'). Css ({'border-color':'#3a87ad', 'color':'#fff'}) .on ('ጠቅ', ተግባር () {
                $(this).text ('አጠናቅቅ ውጤት'); በ ('ጠቅ');
                endQuiz ();
            })

        } ሌላ ቢሆን (የአሁኑ ጥያቄ &lt; quiz.length) {
            $ ('# submitbutton'). Html ('NEXT QUESTION &amp;raquo;') removeClass ('btn-success'). AddClass ('btn-warning'). Css ({'font-weight':'bold', 'border-color':'#faa732', 'color':'#fff'}) .on ('ጠቅ ማድረግ' ተግባር () {
                $(this).text ( '- መልስ ፈትሽ -') removeClass ( 'btn-ማስጠንቀቂያ') addClass ( 'btn-ስኬት ») CSS (...{'font-weight':'bold', 'border-color':'#51a351', 'color':'#fff'}) .on (' ጠቅ ');
                nextQuestion ( );
            })
        } ሌላ {
            // $ ( '# submitbutton') HTML ( 'ቀጣዩ ጥያቄ. &amp;raquo;'.) ላይ (, 'ጠቅ' ተግባር () {
            //      $(this).text ( '- መመርመር - '). Css ({'color':'inherit'}) .on (' ጠቅ ');
            //})
        }


    }

    / **
     * ለእያንዳንዱ አዝራር የክስተት አድማጭ ያዘጋጃል.
     * /
    ተግባራት setupButtons () {
        $ ('choice') በ on ('ጠቅ', function () {
            picked = $(this).attr ('data-index');
            $ ('choice'). removeAttr ('style'). off ('mouseout mouseover');
            $(this)css ({'font-weight':'bold', 'border-color':'#51a351', 'color':'#51a351'});
            if (submt) {
                submt = false;
                $ ('# submitbutton'). css ({'color':'#fff','cursor':'pointer'}) .on ( ) (, {ተግባር 'ጠቅ'
                    $ ጠፍቷል ( 'ጠቅ') ( 'ምርጫ.').;
                    $(this).off ( 'ጠቅ');
                    processQuestion (አነሱት);
                });
            }
        })
    }

    / **
     * Quiz ይጠናቀቃል, መልዕክት ያሳዩ.
     * /
    ተግባር endQuiz () {
        $ ('# ማብራሪያ'). ባዶ ();
        $ ('# ጥያቄ'). ባዶ ();
        $ ('# choice-block'). ባዶ ();
        $ ('# submitbutton'). Remove ();
        $ ('rsform-block-submit'). AddClass ('show');
        $ ('# ጥያቄ') የጽሑፍ ("ከ" + "+" ውጤት + "ከ" + quiz.length + "ትክክል").
        $ (document.createElement ('h4')) addClass ('score') ጽሑፍ (Math.round (score / quiz.length * 100) + '%'). Insert after ('# question');         
    }

    / **
     * ለመጀመሪያ ጊዜ ያሂዳል እና ለ quiz
     * /
    ተግባራት መነሻ ንጥል ይፈጥራል () {
        // አርእስት
        ከሆነ (የግጥም ርእስ! == "ያልተወሰነ" &amp;&amp; $. type (quiztitle) === "string") {
            $ (document.createElement ('h2')) .txt (quiztitle) .appendTo ('# frame');
        } // else {
            //$(.document.createElement('h2')).text("Quiz").appendTo ('#frame');
</code></pre>

<p>//}</p>

<pre><code>        // ፕላግ አክል እና ጥያቄዎች
        if (type quiz! == "undefined" &amp;&amp; $ .type (quiz) === "array") {
            / add pager
            $ (document.createElement ('p')) .addclass ('pager'). attr ('id', 'pager') ጽሑፍ ('ጥያቄ 1 of' + quiz.length) .appendTo ('# frame');
            // የመጀመሪያ ጥያቄ
            $ (document.createElement ('h3')). AddClass ('ጥያቄ'). Attr ('id', 'question') .txt (ጥያቄ[0]['question']). «#frame»);
            / ካለ ምስሉ ይጨምሩ
            (ጥያቄ[0].hasOwnProperty ('image') &amp;&amp; quiz[0]['image']! = "") {
                $ (document.createElement ('img')) addClass (' ጥያቄ-ምስል '). attr (' id ',' question-image '). attr (' src ', quiz[0][' image ']). attr (' alt ', htmlEncode (quiz[0][' question ']) ) .appendTo («# frame»);
            }

            $ (document.createElement ('p')). AddClass ('ማብራሪያ'). Attr ('id', 'explanation'). Html ('') appendTo ('# frame');

            // ጥያቄዎችን የያዘ
            $ (document.createElement ('ul')). Attr ('id', 'choice-block').

            / ምርጫዎችን ይጨምሩ
            addChoices (ጥያቄ[0]['ምርጫዎች']);

            / አስገባ የሚለውን አዝራር
            $ (document.createElement ('div')). AddClass ('id', 'submitbutton'). ('- መልስ ሰጪ -' ); css ({'font-weight': 'bold', 'color': '# fff', 'padding': '30px 0', 'border-radius': '10px' ')) appendTo (' # frame ');

            setupButtons ();
        }
    }

    init ();

});

jQuery (ሰነድ) .ready (ተግባር ($) {         
    $ ("# ጥያቄ"). Html (function () {
    var text = $(this).text (). Trim (). Split ("");
    var first = text.shift (),
        return (text.length &gt; 0? "&lt;span class='number'&gt;" + መጀመሪያ + "&lt;/span&gt; ": መጀመሪያ) + ጽሑፍ.join ("");
    });

    $ ( 'p.pager') እያንዳንዱን (ተግባር () {.
        var ጽሑፍ = $(this).text () መከፋፈል ( '.');
        (text.length ከሆነ &lt; 2)
            ; መመለስ

        ጽሑፍ[1] = '&lt;span class="qnumber"&gt;'+ text[1]+'&lt;/span&gt;',
        $(this).html (
            text.join (' ')
        ),
    });

}); 

    functional copyText () {
        var output = document.getElementById ("frame"). InnerHTML;
        document.getElementById ("placecontent"). እሴት = output;
    }

&lt;/script&gt;
&lt;style type="text/css" media="all"&gt;
    ግብዓት {ቁመት: 30 ፒክሰል! አስፈላጊ; }
    ግቤት [ዓይነት = የአመልካች ሳጥን] {ቁመት: 30 ፒክሰል! አስፈላጊ; ኅዳግ-ከፍተኛ: -3 ፒክስል! አስፈላጊ; ህዳግ-ቀኝ: 5 ፒክስል አስፈላጊ; ሳጥን-ጥላ: የለም; የበስተጀርባ-ቀለም: #ffffff; ቦታ: አንጻራዊ ነው! }
    area {ወርድ: 90%; ኅዳግ: 0 መኪና; ማሳያ: አግድ; }
    ግብዓት [አይነት = ሬዲዮ] {ቁመት: 30px! ጠቃሚ; ኅዳግ-ከፍተኛ: -3 ፒክስል! አስፈላጊ; ህዳግ-ቀኝ: 5 ፒክስል አስፈላጊ; ሳጥን-ጥላ: የለም; የበስተጀርባ-ቀለም: #ffffff; ቦታ: አንጻራዊ ነው! }
    -ፎርማት-ቡድን ግቤት, .form-group select {height: 30px; ድብድብ: 0px 12px; }
    ቅርፅ-አግድመት .form-group {margin: 10px; }
    .formContainer .formControlLabel {ስፋት:! ራስ አስፈላጊ; ደቂቃ-ወርድ: 150 ፒክስል; ኅዳግ: 0; ማጣመር: 0; }
    .formControls {ስፋት: 100%; ማጣመር: 0; ኅዳግ: 10px 0 20px ራስ; }
    .radio {padding-ከላይ: 0 አስፈላጊ; padding-left: 8px! important; }
    .radio-የመስመር {ህዳግ-ቀኝ: 10px; padding-top: 0! ጠቃሚ! ማሳያ: መስመር ውስጥ; }
    እደታን {ቅርጸ-ቁምፊ: ደማቅ; }
    .italic {የቅርፀ-ቅጥ: ሰያፍ; }
    .clear {ስፋት: 100%; ማርች: 0 አስፈላጊ; }
    .rsform-የማገጃ-ማስገባት {ማሳያ: none; }
    ትዕይንት {ማሳያ: አግድ! አስፈላጊ; }
</code></pre>

<p>/ * .rsform-block-placecontent {display: none; } * /
        # ማስገባት {margin: 0 ራስ; ማሳያ: አግድ; }</p>

<pre><code>    / * QUIZ STYLES * /
    ol {list-style: none; }
    ኡል # ምርጫ-ማገድ {አምዶች: 4; -webkit-columns: 4; -moz-columns: 4;}
    ጠንካራ {ቅርጸ-ቁምፊዎች 700 }
    # ክፈፍ {ወርድ: ራስ; ከፍተኛ-ስፋት: 800 ፒክስል; ዳራ; ግልጽ; ኅዳግ: 3px ራስ-ሰር; መጋረጃ: 10 ፒክስል; ቀለም: # 333! ጠቃሚ; }
    # ክፈፍ h2 {ወርድ: ራስ; ከታች-ታች: 1px ጠንካራ #bdbdbd; ጥቅል: 0 0 5px 0; ቅርጸ-ቁምፊ-30 ፒክስል; }
    h3.question {font-weight: normal; ኅዳግ: 20px 0; ማጣመር: 0; ቅርጸ-ቅጥ: italic; ማሳያ: አግድ; }
    p.pager {margin: 5px 0 5px; ቀለም: # 999; ጽሑፍ-አሰላለፍ; ቀኝ; }
    .qnumber {font-size: 25px; ቅርጸ-ቁመት: ደማቅ; ቅርጸ-ቅጥ: italic; አቀባዊ-አሰልፍ: ከታች; }
</code></pre>

<p>/ * .number {font-size: 25px; ቅርጸ-ቁመት: ደማቅ; የቅርፀ ቁምፊ-መደበኛ: መደበኛ; ቀጥ ያለ-አመድ: ውርስ; ድርድር-ቀኝ: 10px; } * /</p>

<pre><code>    . score {width: 100%; ማሳያ: የመስመር ውስጥ ማቆሚያ; ኅዳግ: 30px 0; ቅርጸ ቁምፊ-መጠን: 100 ፒክስል; ጽሑፍ-አሰላለፍ; መሃል; }
    img.question-image {width: 100%; ቁመት: መኪና; ማሳያ: አግድ; ከፍተኛ-ስፋት: 705px; ኅዳግ: 10px ራስ; ክፈፍ: 1px ጠንካራ #ccc; }
* / # ምርጫ-ማገድ {ማሳያ: እገዳ; list-style: ምንም; ኅዳግ: 0; ማጣመር: 0; ጠቋሚ: ጠቋሚ; }
    # መርሃግብሮች {ጠቋሚ: ጠቋሚ; -ዌብ-ኪት-ድንበር-ራዲየስ: 5px; -ሞዝ-ድንበር-ራዲየስ: 5 ፒክስል; የጠርዝ-ራዲየስ 5 ፒክስል; } * /
/ * #submitbutton: hover {background: # 7b8da6; } * /
    # ማብራርያ {ወርድ: ራስ; ደቂቃ-ቁመት: 100 ፒክስል; ኅዳግ: 0 መኪና; መጋረጃ: 20 ፒክስል 0; ጽሑፍ-አሰላለፍ; መሃል; }
    # ማብራሪያ ማብራሪፊ {ቅርጸ-ቁምፊ: ደማቅ; መታገድ-ቀኝ: 8px; }
    ቅቤ-ሳጥን {ስፋት: 50%; ማሳያ: አግድ; ጽሑፍ-አሰላለፍ; መሃል; ኅዳግ: 5px ራስ! አስፈላጊ; ማሸጊያ: 10 ፒክሰል 0 አስፈላጊ! ክፈፍ: 1px ጠንካራ #bdbdbd; }
    ትክክለኛ {ቀለም: # 51a351; ቅርጸ-ቁምፊ-20 ፒክስል; ማሳያ: አግድ; ኅዳግ-ታች 5 ፒክስል; ከታች-ታች: 1px # 51a351 ጠንካራ; ድብዳብ-ታች: 5px; }
    ትክክል አይደለም {ቀለም: # f93939; ቅርጸ-ቁምፊ-20 ፒክስል; ማሳያ: አግድ; ኅዳግ-ታች 5 ፒክስል; ከታች-ታች: 1px # f93939 ጠንካራ; ድብዳብ-ታች: 5px; }
&lt;/style&gt;
</code></pre>

<p></head>
<body></p>

<div class="form-group rsform-block rsform-block-framecontent">
    <div id="frame" role="content"></div>
</div>

<hr>

<!--<div class="form-group rsform-block rsform-block-placecontent">
    <label class="col-sm-3 control-label formControlLabel" data-toggle="tooltip" title="" for="placecontent"></label>
    <div class="col-sm-6 formControls">
        <textarea cols="50" rows="5" name="form[placecontent]" id="placecontent" readonly="" class="rsform-text-box form-control rsform-text-box"></textarea>           
    </div>
</div>  -->

<p><!--<div class="col-sm-6 formControls rsform-block-submit">
    <button type="submit" name="form[submit]" id="submit" onclick="copyText()" class="rsform-submit-button  btn btn-primary">Submit Quiz</button>           
</div> -->
</body>
</html></p>

<p><em>ይህ ጥያቄ በኢንተርኔት ኤክስፕሎረር ውስጥ አይሰራም. ጥያቄውን ማየት ካልቻሉ እባክዎ ሌላ አሳሽ ይሞክሩ.</em></p>
</script>