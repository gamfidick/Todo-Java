# imprimir-la-serie-Fibonacci
# JAVA FRAMES
 // TODO add your handling code here:
        int N; // --- Nro. de Terminos
        int Previo=0;
        int Actual=1;
        int Siguiente;
        String Texto;
        String Cadena="";
        // --- Leer Numero de Terminos
        N = Integer.parseInt(txtNumeroTerminos.getText());
        // --- Determinar la serie fibonacci
        for(int K=1; K <= N; K++)
        {
        Cadena = Cadena + " " + Actual;
        Siguiente = Previo + Actual;
        Previo = Actual;
        Actual = Siguiente;
        }
        // --- Escribir la serie fibonacci
        Texto = "NUMERO DE TERMINOS" + String.valueOf(N)+" MENSAJE"+String.valueOf(Cadena)+ "\n";
         atxMensaje.append(Texto);
