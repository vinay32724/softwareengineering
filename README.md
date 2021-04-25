This README is for illustrating different process adhered in Software Engineering

      
      function int allow_transfer(sender_balance, receiver_account, amount_to_be_sent){

            if(amount_to_be_sent > sender_balance){ 
                     return ERR.INSUFFICITENT_BAL;
              }
            
            if(receiver_account.beneficiary_status != "ACTIVE"
                    return ERR.BENEFICIARY_INACTIVE;
             }
            
             return TRANSFER_ALLOWED;
             
        }
             

    public void test_Transfer()
    {
        receiver_account rc1 =  receiver_account(beneficiary.status = "ACTIVE") 
        int result1 = allow_transfer(sender_balance = 1000, receiver_account = rc, amount_to_be_sent = 5000)
        Assert.AreEqual(ERR.INSUFFICITENT_BAL, result);
        
        receiver_account rc2 =  receiver_account(beneficiary.status = "INACTIVE")
        int result2 = allow_transfer(sender_balance = 1000, receiver_account = rc, amount_to_be_sent = 800)
        Assert.AreEqual(ERR.BENEFICIARY_INACTIVE, result);
        
        receiver_account rc3 =  receiver_account(beneficiary.status = "ACTIVE")
        int result3 = allow_transfer(sender_balance = 1000, receiver_account = rc, amount_to_be_sent = 800)
        Assert.AreEqual(TRANSFER_ALLOWED, result);
    }
