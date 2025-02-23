# Recursive-CTE-Ki-Sabse-Aasaan-Misal-Step-by-Step

Socho tum ek dost ko phone karte ho, lekin wo tumhe jawab nahi deta. Tum dubara call karte ho, phir bhi jawab nahi aata.
Tum bar bar call karte rehte ho, jab tak wo jawab na de ya tum 10 baar call na kar lo.

🚀 Yahi Recursive CTE ka concept hai!

SQL ek query ko repeat karta rehta hai jab tak stopping condition na mil jaye.

Asaan Example: Ginti 1 Se 10 Tak

    WITH Counting AS (
    -- Pehla number (Base Case)
    SELECT 1 AS num  
    UNION ALL  
    
    -- Agla number add karo (Recursive Case)
    
    SELECT num + 1  
    FROM Counting  
    WHERE num < 10  -- Jab tak 10 na aa jaye, chalta rahe
    )
    
    SELECT * FROM Counting;




