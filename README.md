# matriz
matriz
public static void main(String[] args)  
    {  
        int[][] matriz = new int[3][3];  
        Vector v = new Vector();  
        for (int i = 0; i &lt; matriz.length; i++)  
        {  
            matriz[i][i] = 1;  
        }  
        for (int i = 1; i &lt; matriz.length; i++)  
        {  
            for (int j = 0; j &lt; matriz.length - i; j++)  
            {  
                matriz[j][i+j] = 0;  
                v.add(matriz[j][i+j]);  
            }  
        }  
        for(int i = 0; i &lt; matriz.length; i++)	{
        	for(int j = 0; j &lt; matriz[i].length; j++)	{
        		System.out.print(matriz[i][j]);
        	}
        	System.out.println(&quot;&quot;);
        }
    }
