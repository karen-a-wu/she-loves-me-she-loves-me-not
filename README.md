<h1>She Loves Me... She Loves Me Not 🌼💔</h1>
<p>My attempt at an application that evaluates interest level based on texting behavior in dating (mainly for online dating) 😂 <br> <b>This is just for fun and does not provide a definitive answer, as we all know that human relationships are very nuanced and cannot always be quantified accurately.</b></p>
<h2>How This All Works - The Mathematical Model Behind It</h2>
<p>I first developed a VERY SIMPLISTIC mathematical model that estimates a girl's level of interest based on texting behavior. To do so, I tried my best to think of definitive signs that a girl has a strong interest in you... whatever "strong" means - maybe at least a crush? Not just things she may do that may indicate a stronger interest in you, like how most dating advice go. But actual signs that definitively prove 💯 that a girl has interest in you. Please note that I thought of these signs in the context of meeting someone through online dating, as opposed to in-person, cold-approach dating (yes, that matters).</p>
<p>Anyways, below are the model parameters that take into account the signs I have thought of.</p>
<h3>Thoughtfulness Score (TS)</h3>
<p>Measures the depth and personal nature of her responses.<br>
<b>Formula:</b> (Number of texts with personal details + Number of texts with personal questions) / Total number of texts<br>
<b>Range: </b>0 (least thoughtful) to 1 (most thoughtful)</p>
<h3>Initiation Frequency (IF)</h3>
<p>Indicates how often she initiates conversation.<br>
<b>Formula:</b>  Number of initiated conversations by her / Total number of conversations<br>
<b>Range: </b>0 (never) to 1 (always)</p>
<h3>Response Time (RT)</h3>
<p>Measures the average time she takes to respond, with a focus on the 6-8 hour window as an interest threshold (anything over 6-8 hours indicates low interest).<br>
<b>Formula:</b> Sum of response times / Number of responses.<br>
<b>Ranges: </b> <br>
If RT ≤ 6 hours: Score = 1 (high interest)<br>
If 6 hours < RT ≤ 8 hours: Score is scaled linearly between 1 and 0.5. <br>
If RT > 8 hours: Score = 0 (low interest)<br></p>
<h3>Interest in Meeting Up (IM)</h3>
<p>Binary parameter indicating if she shows explicit intent to meet up (1 for yes, 0 for no).</p>
<h3>Conversational Balance Score (CS)</h3>
<p>The app will ask you to rate the balance and mutual enthusiasm in the conversations on a scale of 1-5.<br>
<b>Range: </b>1 (lowest balance and mutual enthusiasm - conversations are heavily one-sided or lacking in engagement) to 5 (highest balance and mutual enthusiasm - the conversation consistently exhibits equal engagement and interest from both parties)</p>
<h3>Response Length (RL)</h3>
<p>Average length of her messages.<br>
<b>Formula:</b> Sum of the length of messages / Number of messages<br>
<h3>Overall Interest Score (OIS)</h3>
<p>A summative assessment of her interest in you.<br>
<b>Formula:</b> (TS + IF + RT + IM + Normalized CS) / 5, where Normalized CS = (CS - 1) / 4<br>
<b>Range: </b>0 to 1 (higher score indicates higher interest)</p>
<h2>Determining Fluctuation in Interest</h2>
<p>I also wanted to include whether her interest in you is increasing or decreasing.<br>
<h3>Change in Response Time (ΔRT)</h3>
