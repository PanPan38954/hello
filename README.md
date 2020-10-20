# hello
i dont know what i am doing here oof
print("Title of program: Encouragement bot")
print()
while True:
  description = input("Could you describe how you feel in a sentence?")

  list_of_words = description.split()

  feelings_list = []
  encouragement_list = []
  counter = 0
  
  for each_word in list_of_words:
    
    if each_word == "sad":
      feelings_list.append("sad")
      encouragement_list.append("we can both be the depression brothers")
      counter += 1
    if each_word == "happy":
      feelings_list.append("happy")
      encouragement_list.append("why are you happy your are supposed to be depressed stupid boy")
      counter += 1
    if each_word == "tired":
      feelings_list.append("tired")
      encouragement_list.append("good to know that you are a weakling")
      counter += 1

  if counter == 0:
    
      output = "can you use real words. or are you so stupid that you do not even know what to say?"

  elif counter == 1:
    
      output = "It seems that you are feeling quite " + feelings_list[0] + ". However, do remember that "+ encouragement_list[0] + "! Hope you feel better :)"  

  else:

    feelings = ""    
    for i in range(len(feelings_list)-1):
      feelings += feelings_list[i] + ", "
    feelings += "and " + feelings_list[-1]
    
    encouragement = ""    
    for j in range(len(encouragement_list)-1):
      encouragement += encouragement_list[i] + ", "
    encouragement += "and " + encouragement_list[-1]

    output = "It seems that you are feeling quite " + feelings + ". Please always remember "+ encouragement + "! Hope you feel better :)"

  print()
  print(output)
  print()

