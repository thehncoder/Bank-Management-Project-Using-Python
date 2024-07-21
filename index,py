name=[]
pin=[]
money=[]
while True:
    print("====WELCOME TO CAPITAL BANK====")
    print("====1.OPEN A NEW ACCOUNT   ====")
    print("====2.DEPOSIT MONEY        ====")
    print("====3.WITHDRAW CASH        ====")
    print("====4.SEE CUSTOMER DETAILS ====")
    print("====5.EXIT                 ====")
    c=int(input("ENTER YOUR CHOICE"))
    if c==1:
        n=input("ENTER YOUR FULL NAME")
        na=n.upper()
        p=int(input("CREATE A 4 DIGIT PIN"))
        ps=len(str(p))
        while ps!=4:
            p=int(input("PLS CREATE A 4(FOUR) DIGIT PIN"))
            ps=len(str(p))
        m=int(input("ENTER VALUE TO DEPOSIT IN YOUR ACCOUNT"))
        print("(:DEAR,",na,"YOUR ACCOUNT IS CREATED SUCCESSFULLY :)")
        print("  YOUR CURRENT ACCOUNT BALANCE IS RS",m)
        print("  YOUR ACCOUNT PIN IS-",p)
        print("  PLS REMEMBER YOUR PIN")
        name.append(na)
        pin.append(p)
        money.append(m)
    elif c==2:
         N=input("ENTER YOUR NAME")
         NA=N.upper()
         P=int(input("ENTER YOUR PIN"))
         if NA in name:
             if P == pin[name.index(NA)]:
                 deposit=int(input("ENTER VALUE TO DEPOSIT"))
                 money.pop(name.index(NA))
                 m=deposit+m
                 print("YOUR CURRENT ACCOUNT BALNCE IS RS-",m)
                 money.insert(name.index(NA),m)
            
             else:
                print("PIN DONT MATCH")
         else:
             print("NAME NOT FOUND")
    elif c==3:
        N=input("ENTER YOUR NAME")
        NA=N.upper()
        P=int(input("ENTER YOUR PIN"))
        if NA in name:           
            if P == pin[name.index(NA)]:
                b=money[name.index(NA)]
                print("YOUR AVAILABLE BALANCE IS RS-",b)
                w=int(input("ENTER VALUE TO WITHDRAW:)"))
                if b>=w:
                    print("==WITHDRAW SUCCESSFUL==")
                    B=b-w
                    print("YOUR CURRENT ACCOUNT BALNCE IS RS-",B)
                    money.pop(-1)                    
                    money.append(B)                    
                    m=B                  
                else:
                    print("INSUFFICIENT BALANCE")
            else:
                print("PIN DONT MATCH")
        else:   
            print("NAME NOT FOUND")
    elif c==4:
        print("NAME-",(name))
        print("PINS-",(pin))
        print("MONEY(IN RS)-",(money))
    elif c==5:
        print("=====::THANKS FOR USING::=====")
        print(":):):):):):):):):):):):):):):)")
        exit()
    else:
        print("=====INVALID CHOICE===QUITTING NOW====")
        quit()
