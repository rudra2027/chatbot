# chatbot
from nltk.chat.util import Chat,reflections

pairs=[
    ['my name is (.*)',['hi! %1']],
    ['(hi|holla|heya|hey|hello)',['hey there!how may i help you?']],
    ['(.*)in(.*)is fun',['%1 in %2 is indeed fun ']],
    ['(.*) ete',['ete:-weightage is fifty percent; try to score enough.what else?']],
    ['(.*) mte',['mte:-weightage is twenty percent;try easy.what else?']],
    ['(.*) ca',['ca:-weightage is twenty five percent;try to score as best as possible.what else?']],
    ['(.*) attendance',['atten.:-weightage is five percent;mandatory :- seventy five plus percent.what else?']],
    ['(.*) exam schedule',[' you will know it via ums or lpu touch.anything else i can help with?']],
    ['ok',['yups, anything else?']],
    ['yes',['may i know?']],
    ['sure',['go on..']],
    ['(.*) path',['sure! ums- login >home>ums navigation>examination>time table','for lpu touch:-lputoch>exams available']],
    ['(.*) (do not|did not)',[' score well in rest of examinations and specially in ca,also manage proper attendance.']],
    ['(.*) backlog',['factors:more than ten percent in mte,more than twenty percent in ete,more then fourty percent overall/subject,umc back']],
    ['(.*) umc back',['in case you were found disrespecting laws/ rules & regulation of university you are bearer of umc that undefines your  scholarship as well as if serious  you maybe  backed']],
    ['(.*) come to know our result or marks',['you will recieve lpu touch notification regarding that.']],
    ['(.*)  too see my answer sheets',[' regarding scrutiny of sheets -respective authorities will inform you although its for written sheets not mcq based.']],
    ['no',['thank you,had a great conversation.have a good day ahead!']],
    ['(.*) thank you',['thank you,had a great conversation.have a good day ahead!']],
    #giving a general query convo. can be eddited as per requirements.
    


]

reflections

my_dummy_reflections={
    'go':'gone',
    'hello':'hey there'
}

chat=Chat(pairs,my_dummy_reflections)
#chat._substitute(' go hello')
chat.converse()

