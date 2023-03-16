# WPFThreads
## Argomenti del progetto
### -Uso delle Lambda Expression: 
Questa espressione è una sorta di metodo che fornisce un elenco di dei parametri in un blocco di codice. L'espressione lambda permette di ridurre delle linee di codice da scrivere.
### -Uso e le motivazioni del costrutto C# lock:
#### Abbiamo messo
        void Incrementare()
        {
            for(int x = 0; x < NGIRI; x++)
            {
                _counter++;
                Dispatcher.Invoke(
                    () =>
                    {
                       counter1.Text = _counter.ToString();
                    }
                );
                Thread.Sleep(1);
            }
        }
        
