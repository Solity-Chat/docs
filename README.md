# Dabatabase model

> User:
  - user_id: Number
  - user_name: String
  - user_bio: String
  - user_is_active: Bool
  
> Conversation
  - conversation_id: Number
  - number_of_messages: Number

> Message
  - user_id_recv: Number
  - user_id_snd: Number
  - message_content: String
  - message_status: Int
  - conversation_id: Number
  
  Encrypt on server / user
  
  message_clean -> message_encrypted_popescu {micro backend local} -> server -> {process} -> send_to_receiver -> 
  encrypted_message -> before_display_decrypt 
  
  Electron -> server -> Electron 
  
> SSH key
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAACAQDDRKcmia27PVmE6B5siZ57tHjoUyO++w1ICJmHnUFRn1Iz8ViKUKx3Zqk0DkXvjNek0z5VkAdBw20cl4KWMHpsIl30Z2EcKyGdM+fo0d6Prv1CsFEL8oC35wnM4TEXDLHNDsU/UJsvekizuXhmPmhjCCs5rbHDWPDWn7bX26ubyYBA21hs1eo9f+nceit+KVMHPOpATKUL7ikJHPbgTASPr46r0MbVj1UqfqzWK74tA4vcl9XwLRLrVMMUuEwV9VOqt3ew/fHo46PBy1LQdWpSXCxCDzJQJEhM9P9Nai+wgYGpBczjD4X+b33S1am5MheJPiTMj7ATfunUD6uAOKbCHEoLJSqpLNBikKXxr1gxjsI0Lp1lQR7sg53GIbBCAOdYnyWLKL1GzbDzsimW1otIuuoA7BJCiM1+Zilhcltl7OMVP5wOIhJnaaGPkOfRwikLa/5wylQ2HL4McJm6XvHAxnZ6+f9yVDkCpfqMGvv8Os6jvQ2VRAAVJE6mrk+TeBhuMR4oOKgjcTUU2PHe0IbTJfKr/dltfIzpYfm+wYOxpq3S9iQc2arx1QmQzqCshYl1RK2onvqnUteFDy0D3tFuQL6iIf4ABBQs+MdgymKNN6J8rN9/7maoQyxUjyG3e5YRIWdIPBzV7eVeOfrHlIdDBFPHJJnFbz6mtCEpCjLx/w== root+830453045970@cloud9.amazon.com

