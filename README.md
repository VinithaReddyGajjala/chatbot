{ 
"name": "AskInterest", 
"type": "slot", 
"variable": "interestArea", 
"question": { 
"text": "What subject are you interested in? (e.g., AI, Web Development, Cybersecurity)" 
}, 
"next_step": { 
"behavior": "jump_to", 
"dialog_node": "AskLevel" 
} 
} 

<!DOCTYPE html> 
<html lang="en"> 
<head> 
<meta charset="UTF-8"> 
<title>Course Recommendation Bot</title> 
<style> body { font-family: 'Segoe UI', sans-serif; 
margin: 0; 
background: linear-gradient(135deg, #f1f9ff, #e0f2f1); 
} header { background-color: #004d99; 
color: white; 
padding: 20px; 
text-align: center; 
} 
.container { text-align: center; 
padding: 50px; 
} 
.container h2 { font-size: 2em; margin-bottom: 20px; 
} 
.container p { font-size: 1.2em; color: #444; 
} footer { text-align: center; font-size: 0.9em; padding: 20px; background-color: #f2f2f2; margin-top: 80px; 
} 
</style> 
</head> 
<body> 
<header> 
<h1>Course Recommendation Bot</h1> 
</header> 
 
<div class="container"> 
<h2>Welcome!</h2> 
<p>Interact with our AI chatbot below to receive personalized course suggestions based on your interests and background.</p> 
</div> 
 
<footer> 
&copy; 2025 Tejaswi – B.Tech CSE Core | VIT | GENAI Project </footer> 
 
<!-- C˛* IBM Watson Assistant Integration --> 
 
<script> window.watsonAssistantChatOptions = { integrationID: "fb18aedf-766e-4bb4-866c-703e5d74e049", // The ID of this integration. region: "us-south", // The region your integration is hosted in. 
serviceInstanceID: "069e48cc-1702-471d-8e5c-15097daba302", // The ID of your service 
instance. 
onLoad: async (instance) => { await instance.render(); } 
}; setTimeout(function(){ 
const t=document.createElement('script'); 
t.src="https://web-chat.global.assistant.watson.appdomain.cloud/versions/" + 
(window.watsonAssistantChatOptions.clientVersion || 'latest') + 
"/WatsonAssistantChatEntry.js"; document.head.appendChild(t); 
}); 
</script> 
</body> 
</html> 
