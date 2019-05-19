# Projet Ul - Lift up

>Lift up has been designed and designed for people with mild motor disabilities. Many people can not or have difficulty getting up when sitting on a chair, so for those people, we wanted to create a prototype chair and look like a regular chair. which could be placed in the restaurants so that people can eat at the restaurant without help to get up. This project is very important to us and we will explain our thoughts, our motivations and its progress.

[Presentations slide](https://docs.google.com/presentation/d/1F90I4jqLM0xJeXBUU_vE5x2pX4bnX4WyPgPFGB-84LE/edit?usp=sharing)


## Présentation


__Lift up__ a été imaginée et conçue pour les personnes avec _un léger handicap moteur_. Beaucoup de personne ne peuvent pas ou ont du mal à se relever lorsque qu'ils sont assis sur une chaise, et donc pour ces personnes là, on a voulu créer un prototype de chaise autonome et a l'aspect d'une chaise ordinaire __qui pourrait donc être placé dans les restaurants__ pour que ces personnes puissent manger au restaurant __sans aide pour se relever__.

Pourquoi somme nous aller vers ce projet ? __Ici je vais parler personnellement (Richard)__ je connais plusieurs personnes qui souffre au niveau des jambes, et ce qui m'a le plus marqué c'est mon grand-père qui aime beaucoup sortir aux restaurents mais depuis quelques années il ne veut plus y aller car il se __sent gênez de demander de l'aide pour le relever d'une chaise__, comme il existe déjà des siège et fauteuils qui aide à se relever, pourquoi des chaises fine ne peuvent pas le faire aussi ? En partant de cette question, le projet est né et les schémas ont commencé à être imaginé.


## Choix du Projet


Il y avait plusieurs styles de chaise possible, la première aurais étais de faire __une chaise totalement automatisée avec des rails__ pour que les personnes n'aient pas grand chose à faire et surtout qu'il n'est pas à forcer, sauf que ce type avait des défauts, elle aurait étais __très peu maniable__ pour les restaurateurs et les rails aurais pu fait tomber une personne. Donc personnes ne l'auraient acheté.

Un version similaire a vu le jour dans nos tête juste après, __remplacer les rails par des roues__, sauf que comme l'exemple du grand-père de richard, il a honte qu'on le voit avoir besoin d'aide, donc voir des roue sous une chaise serais la preuve qu'il a besoin d'aide. Mais aussi des problèmes techniques, car il faudrait gérer les roues pour éviter que la chaise glisse ou se retourne due à un centre de gravité mal gérée. Et si les roues étaient motorisées, il faudrait vérifier s'il y a un obstacle derrière la chaise et si oui, ne pas reculer. On est donc partie sur le troisième modèle qui est qu'on __garde l'architecture basique d'une chaise__, on rajoute un moteur ou des piston en dessous les plus discrets possibles, la personne devras certes faire un peu plus d'effort que les 2 autres chaises citez au-dessus, mais __la chaise sera pratiquement la même que les autres dans le restaurant__, et c'est vraiment le __but du projet__.

Bon, partant de cette idée, on avait deux choix qui s'ouvrait a nous :
* Faire une maquette puis essayer de faire une chaise grandeur nature. 
* Faire un prototype fonctionnel pour sa taille.

On est partie pour un prototype fonctionnelle, car nous n'avions ni le temps, ni les moyens financiers pour un tel projet. 


## Brainstorm


Le projet étais donc lancer, nous avons quand même regarder sur le net si des chaise de ce style exister dans le marché. Mais sans grande trouvaille, sauf un produit nous reste en tête 
[Coussin d'aide à la levée](https://www.tousergo.com/aide-au-transfert/28-coussin-d-aide-a-la-levee-3574590140219.html).
Comme prévue pratiquement, aucune société ne fait de chaise de ce style, les sociétés préfèrent viser le marché des fauteuils par rapport aux chaises.

Nous avons réfléchi à plusieurs idées permettant de faire monter le siège d'une chaise :

1. La première idée fut les pistons, simples.
2. La deuxième était de passer par une [vis sans fin](https://upload.wikimedia.org/wikipedia/commons/b/b8/Vis100f1.png) qui est un engrenage et une vis.  
3. La troisieme était de passer via un engrenage et une crémaillère, moins robuste, mais efficace.

La première est très efficace, mais chère et dangereuse si elle est mal programmer (elle pourrait catapulter la personne contre la table ou son voisin d'en face). La deuxième peut soulever une importante charge et de manière précise. Mais est impossible due à l'irréversibilité de la vis sans fin, car on ne pouvait pas placer la vis de la manière voulue due a la présence du moteur qui bloquait la crémaillère. La troisième est fonctionnelle et efficace, mais dépendante de la matière dont est constituer la crémaillère ainsi qu'a la fixation entre la crémaillère et l'assise de la chaise. Car si le poids et trop important, soit la crémaillère cède sous le poids ou bien la crémaillère perfore l'assise si la force sur l'assise de la chaise est mauvaise.  

Nous avons donc choisit de passer par la troisième méthode.

![](https://zupimages.net/up/19/20/yr36.png) ![](https://zupimages.net/up/19/20/filr.png) ![](https://zupimages.net/up/19/20/6vpy.png)

## Fabrication

### Construction

Pour commencer, il nous fallait fabriquer une chaise pour le prototype, mais nous n'avions pas assez de temps. Nous avons donc plutôt opté pour une [chaise en kit](https://www.ikea.com/fr/fr/p/kritter-chaise-enfant-rouge-80153697/) de chez IKEA.
Nous avons donc modifier la chaise de manière a retirer les vises qui maintenait l'assise. Et nous les avons remplacé par des charnières qui permettent à la chaise de se lever tout en restant fixer au squelette de la chaise. 

Comme c'est un prototype, il se doit d'être peu coûteux. Donc nous avons choisi de fabriquer la crémaillère en plastique imprimer avec une imprimante 3D. L'engrenage a aussi été imprimé en 3D pour qu'il s'emboîte parfaitement. Anis qu'un bloc pour les contenir et qu'il reste assembler.Les pièces étant uniques nous avons due les modéliser en 3D, c'est Aziz qui la fait. Vous pouvez voir [ici](https://www.tinkercad.com/things/dY0HXlwu65n) les pièces modélisées pour le premier test et [ici](https://www.tinkercad.com/things/2Bs0kqwbqwV) les pièces utiliser pour le montage final. Seules ces dernières on été imprimer.



### Programmation

Lors de l'avancement une partie programmation étais présente. Nous avons dû programmer de l'Arduino (qui est proche du C et du C++), comme nous ne sommes pas expert en Arduino, nous avons commencé à regarder les librairies disponibles pour le fonctionnement d'un servomoteur, et surtout du Bluetooth.

Suite à plusieurs dizaines d'heures à essayer de faire fonctionner le Bluetooth sur la carte Arduino, même avec l'aide d'un professeur, la carte ne voulais rien savoir. Nous avons mis en place une application Android qui n'a pas abouti, car au début, on croyait que le fait que l'Arduino ne recevait pas les données venais de notre application

`    public class MainActivity extends AppCompatActivity {
        private TextView mBluetoothStatus;
        private TextView mReadBuffer;
        private Button mScanBtn;
        private Button mOffBtn;
        private Button mListPairedDevicesBtn;
        private Button mDiscoverBtn;
        private BluetoothAdapter mBTAdapter;
        private Set<BluetoothDevice> mPairedDevices;
        private ArrayAdapter<String> mBTArrayAdapter;
        private ListView mDevicesListView;
        private CheckBox mLED1;

        private Handler mHandler;
        private ConnectedThread mConnectedThread;
        private BluetoothSocket mBTSocket = null;

        private static final UUID BTMODULEUUID = UUID.fromString("00001101-0000-1000-8000-00805F9B34FB");


        private final static int REQUEST_ENABLE_BT = 1;
        private final static int MESSAGE_READ = 2;
        private final static int CONNECTING_STATUS = 3;

        @Override
        protected void onCreate(Bundle savedInstanceState) {
            super.onCreate(savedInstanceState);
            setContentView(R.layout.activity_main);
            mBluetoothStatus = (TextView)findViewById(R.id.bluetoothStatus);
            mReadBuffer = (TextView) findViewById(R.id.readBuffer);
            mScanBtn = (Button)findViewById(R.id.scan);
            mOffBtn = (Button)findViewById(R.id.off);
            mDiscoverBtn = (Button)findViewById(R.id.discover);
            mListPairedDevicesBtn = (Button)findViewById(R.id.PairedBtn);
            mLED1 = (CheckBox)findViewById(R.id.checkboxLED1);

            mBTArrayAdapter = new ArrayAdapter<String>(this,android.R.layout.simple_list_item_1);
            mBTAdapter = BluetoothAdapter.getDefaultAdapter();

            mDevicesListView = (ListView)findViewById(R.id.devicesListView);
            mDevicesListView.setAdapter(mBTArrayAdapter);
            mDevicesListView.setOnItemClickListener(mDeviceClickListener);




            mHandler = new Handler(){
                public void handleMessage(android.os.Message msg){
                    if(msg.what == MESSAGE_READ){
                        String readMessage = null;
                        try {
                            readMessage = new String((byte[]) msg.obj, "UTF-8");
                        } catch (UnsupportedEncodingException e) {
                            e.printStackTrace();
                        }
                        mReadBuffer.setText(readMessage);
                    }

                    if(msg.what == CONNECTING_STATUS){
                        if(msg.arg1 == 1)
                            mBluetoothStatus.setText("Connected to Device: " + (String)(msg.obj));
                        else
                            mBluetoothStatus.setText("Connection Failed");
                    }
                }
            };

            if (mBTArrayAdapter == null) {
                mBluetoothStatus.setText("Status: Bluetooth not found");
                Toast.makeText(getApplicationContext(),"Bluetooth device not found!",Toast.LENGTH_SHORT).show();
            }
            else {

                mLED1.setOnClickListener(new View.OnClickListener(){
                    @Override
                    public void onClick(View v){
                        if(mConnectedThread != null) //First check to make sure thread created
                            mConnectedThread.write("1");
                    }
                });


                mScanBtn.setOnClickListener(new View.OnClickListener() {
                    @Override
                    public void onClick(View v) {
                        bluetoothOn(v);
                    }
                });

                mOffBtn.setOnClickListener(new View.OnClickListener(){
                    @Override
                    public void onClick(View v){
                        bluetoothOff(v);
                    }
                });

                mListPairedDevicesBtn.setOnClickListener(new View.OnClickListener() {
                    @Override
                    public void onClick(View v){
                        listPairedDevices(v);
                    }
                });

                mDiscoverBtn.setOnClickListener(new View.OnClickListener(){
                    @Override
                    public void onClick(View v){
                        discover(v);
                    }
                });
            }
        }

        private void bluetoothOn(View view){
            if (!mBTAdapter.isEnabled()) {
                Intent enableBtIntent = new Intent(BluetoothAdapter.ACTION_REQUEST_ENABLE);
                startActivityForResult(enableBtIntent, REQUEST_ENABLE_BT);
                mBluetoothStatus.setText("Bluetooth enabled");
                Toast.makeText(getApplicationContext(),"Bluetooth turned on",Toast.LENGTH_SHORT).show();

            }
            else{
                Toast.makeText(getApplicationContext(),"Bluetooth is already on", Toast.LENGTH_SHORT).show();
            }
        }

        @Override
        protected void onActivityResult(int requestCode, int resultCode, Intent Data){
            if (requestCode == REQUEST_ENABLE_BT) {
                // Make sure the request was successful
                if (resultCode == RESULT_OK) {
                    mBluetoothStatus.setText("Enabled");
                }
                else
                    mBluetoothStatus.setText("Disabled");
            }
        }

        private void bluetoothOff(View view){
            mBTAdapter.disable(); 
            mBluetoothStatus.setText("Bluetooth disabled");
            Toast.makeText(getApplicationContext(),"Bluetooth turned Off", Toast.LENGTH_SHORT).show();
        }

        private void discover(View view){
            if(mBTAdapter.isDiscovering()){
                mBTAdapter.cancelDiscovery();
                Toast.makeText(getApplicationContext(),"Discovery stopped",Toast.LENGTH_SHORT).show();
            }
            else{
                if(mBTAdapter.isEnabled()) {
                    mBTArrayAdapter.clear(); 
                    mBTAdapter.startDiscovery();
                    Toast.makeText(getApplicationContext(), "Discovery started", Toast.LENGTH_SHORT).show();
                    registerReceiver(blReceiver, new IntentFilter(BluetoothDevice.ACTION_FOUND));
                }
                else{
                    Toast.makeText(getApplicationContext(), "Bluetooth not on", Toast.LENGTH_SHORT).show();
                }
            }
        }

        final BroadcastReceiver blReceiver = new BroadcastReceiver() {
            @Override
            public void onReceive(Context context, Intent intent) {
                String action = intent.getAction();
                if(BluetoothDevice.ACTION_FOUND.equals(action)){
                    BluetoothDevice device = intent.getParcelableExtra(BluetoothDevice.EXTRA_DEVICE);
                    mBTArrayAdapter.add(device.getName() + "\n" + device.getAddress());
                    mBTArrayAdapter.notifyDataSetChanged();
                }
            }
        };

        private void listPairedDevices(View view){
            mPairedDevices = mBTAdapter.getBondedDevices();
            if(mBTAdapter.isEnabled()) {
                for (BluetoothDevice device : mPairedDevices)
                    mBTArrayAdapter.add(device.getName() + "\n" + device.getAddress());

                Toast.makeText(getApplicationContext(), "Show Paired Devices", Toast.LENGTH_SHORT).show();
            }
            else
                Toast.makeText(getApplicationContext(), "Bluetooth not on", Toast.LENGTH_SHORT).show();
        }

        private AdapterView.OnItemClickListener mDeviceClickListener = new AdapterView.OnItemClickListener() {
            public void onItemClick(AdapterView<?> av, View v, int arg2, long arg3) {

                if(!mBTAdapter.isEnabled()) {
                    Toast.makeText(getBaseContext(), "Bluetooth not on", Toast.LENGTH_SHORT).show();
                    return;
                }

                mBluetoothStatus.setText("Connecting...");
                String info = ((TextView) v).getText().toString();
                final String address = info.substring(info.length() - 17);
                final String name = info.substring(0,info.length() - 17);
                new Thread()
                {
                    public void run() {
                        boolean fail = false;

                        BluetoothDevice device = mBTAdapter.getRemoteDevice(address);

                        try {
                            mBTSocket = createBluetoothSocket(device);
                        } catch (IOException e) {
                            fail = true;
                            Toast.makeText(getBaseContext(), "Socket creation failed", Toast.LENGTH_SHORT).show();
                        }
                        // Establish the Bluetooth socket connection.
                        try {
                            mBTSocket.connect();
                        } catch (IOException e) {
                            try {
                                fail = true;
                                mBTSocket.close();
                                mHandler.obtainMessage(CONNECTING_STATUS, -1, -1)
                                        .sendToTarget();
                            } catch (IOException e2) {
                                Toast.makeText(getBaseContext(), "Socket creation failed", Toast.LENGTH_SHORT).show();
                            }
                        }
                        if(fail == false) {
                            mConnectedThread = new ConnectedThread(mBTSocket);
                            mConnectedThread.start();

                            mHandler.obtainMessage(CONNECTING_STATUS, 1, -1, name)
                                    .sendToTarget();
                        }
                    }
                }.start();
            }
        };

        private BluetoothSocket createBluetoothSocket(BluetoothDevice device) throws IOException {
            return  device.createRfcommSocketToServiceRecord(BTMODULEUUID);
        }

        private class ConnectedThread extends Thread {
            private final BluetoothSocket mmSocket;
            private final InputStream mmInStream;
            private final OutputStream mmOutStream;

            public ConnectedThread(BluetoothSocket socket) {
                mmSocket = socket;
                InputStream tmpIn = null;
                OutputStream tmpOut = null;
                try {
                    tmpIn = socket.getInputStream();
                    tmpOut = socket.getOutputStream();
                } catch (IOException e) { }

                mmInStream = tmpIn;
                mmOutStream = tmpOut;
            }

            public void run() {
                byte[] buffer = new byte[1024];
                int bytes; 
                while (true) {
                    try {
                        bytes = mmInStream.available();
                        if(bytes != 0) {
                            SystemClock.sleep(100); 
                            bytes = mmInStream.available(); 
                            bytes = mmInStream.read(buffer, 0, bytes); 
                            mHandler.obtainMessage(MESSAGE_READ, bytes, -1, buffer)
                                    .sendToTarget(); 
                        }
                    } catch (IOException e) {
                        e.printStackTrace();

                        break;
                    }
                }
            }

            public void write(String input) {
                byte[] bytes = input.getBytes();          
                try {
                    mmOutStream.write(bytes);
                } catch (IOException e) { }
            }
            public void cancel() {
                try {
                    mmSocket.close();
                } catch (IOException e) { }
            }

        }
    }`

Nous avons donc décider d'abandonner le Bluetooth via l'Arduino pour nous consacrer sur le Raspberry, nous avons donc commencer de la programmation python, nous sommes déjà un plus apte à être sur ce langage ayant appris les bases lors de notre année au début le Raspberry servais juste de relais pour envoyer des donner a l'Arduino.

    `#include <Servo.h>

    boolean direction = 0;

    Servo servo_4;

    void setup() {
      pinMode(2, INPUT);
      servo_4.attach(4);
    }

    void loop() {
      if (digitalRead(2) && direction == 0) {
        servo_4.write(180);
        delay(51000);
        servo_4.write(90);
        direction = 1;
      } else if (digitalRead(2) && direction == 1) {
        servo_4.write(0);
        delay(51000);
        servo_4.write(90);
        direction = 0;
      }
      delay(5*1000);

    }`

Pendant le développement du programme en python pour la chaise, nous avons reçu la chaise et nous avons commencer les modifications dessus, pour la rendre "compatible" avec notre système, nous avons troué certain partie, retirer quelques parties aussi, mais nous avons surtout poncer beaucoup de partie que se soit de la chaise ou des pièces imprimé en 3d, rien de très compliquer, ça prend juste un peu de temps et de patience, la chaise avancer donc très bien pendant le temps du développement.

Une première version du code python vu le jour, la chaise se levais et redescendais tout été parfait ! Mais un jour plus rien n'était parfait nous avons donc décider de passer le projet que sur un unique Raspberry et nous avons fait nos adieux à l'Arduino qui nous a poser beaucoup de soucis, mais le Raspberry nous posa aussi beaucoup de soucis, du moins une libraire python nous causa beaucoup de soucis, Même en regardant des tutoriel, des vidéo, la documentation la première libraire que nous avions utilisé été incompréhensible, le moteur ne réagissais pas logiquement. Suite a ça nous avons trouver une nouvelle librairie qui réagissait correctement avec le moteur que nous avions et la chaise été donc enfin fonctionnelle et le fait de passer que par le Raspberry nous fait donc avoir une chaise totalement libre niveau énergie, une simple batterie externe de téléphone suffit pour que la chaise fonctionne.

    `#!/usr/bin/env /usr/bin/python
    from gpiozero import AngularServo
    import time
    import socket

    #pin

    moteur = 18
    up = False

    #setup bleutooth

    server_socket = socket.socket(socket.AF_BLUETOOTH, socket.SOCK_STREAM, socket.BTPROTO_RFCOMM)
    address = "B8:27:EB:8B:31:A9"
    port = 1
    server_socket.bind((address,port))
    server_socket.listen(1)
    print("On standby...")

    client_socket,address = server_socket.accept()
    print("Accepted connection from ", address)

    #moteur

    servo = AngularServo(moteur)

    while True:

        data = client_socket.recv(1024)

        if data == b'0' and up == True:
            print("Down")
            servo.angle = -30
            time.sleep(3)
            up = False

        elif data == b'1' and up == False:
            print("Up")
            servo.angle = 15
            time.sleep(6)
            up = True

        elif data == b's':
            print("Start")
            servo.min()
            time.sleep(5)

        elif data == b'q':
            print("Quit")
            servo.max()
            time.sleep(6)
            servo.angle = 0
            break

        servo.angle = 0 


    #onExit

    client_socket.close()
    server_socket.close()

    from subprocess import call
    call("shutdown -h now", shell=True)`

## Les difficultés

Les plus grosses difficultés rencontrées dans ce projet ont été le caprice que nous a fait l'Arduino, la librairie pas compatible avec notre moteur sur Python, et la modélisation des pièce 3d , pas de grosse difficulté nous on retarder juste des imprévue de temps en temps, mais rien de bien méchant;

La chaise est fonctionelle, mais elle n'est pas parfaite, des améliorations, peuvent etre envisager, que se soit materielle ou même application. Un des premiers ajouts qu'on pourrait faire, c'est un bouton sur la chaise pour donner plus de choix d'utilisation, car les personne agées n'ont pas tous un téléphone, ou même certaine ne savent pas utilisé le Bluetooth, on pourrait aussi créer une télécommande pour simplifier l'utilisation à distance. 

Notre moyen, de faire monter le siège de la chaise n'est pas parfait, il est utile pour les personnes ayant un léger handicap moteur, car la chaise va les aider et ils pourront prendre appuie dès qu'ils le veulent, mais pour les personnes ayant un handicap moteur assez élevé, notre système n'est pas du tout conseillée, car il y a des risques que la personne glisse si ses appuis ne sont pas pris.

Comme prévu n'étant pas des ingénieurs, nous n'avions pas toutes les compétences pour réaliser le projet avec un modèle réel et surtout nous avions pas le budget, la chaise a donc de petit défaut, comme le support moteur qui empêche la fermeture complète de la chaise, car la chaise est trop petite, mais ce souci devrait être réglé si nous passons sur une tailles grandeur nature.

## En Conclusion

Pour conclure, nous sommes fiers de présenter ce projet, c'est un projet qui nous tient a Coeur, essayer de donner une autonomie aux personnes qui la perde suite aux faiblesses de leur corps. C'est un monde qui n'est pas exploiter par les sociétés et nous ne comprenons pas, c'est certes peut être très complexe si on veut associer la puissance des moteur avec l'esthétique d'une chaise et le confort aussi, car il est vrai que nous n'avons pas du tout prêter attention au confort, car nous avions qu'une chaise en bois pour enfant on pouvais pas trop comparais, ce projet prouve que ce n'est pas impossible comme idée et que de nombreuses sociétés pourrais démocratiser ce domaine pour le bien des personnes dans le besoin.
