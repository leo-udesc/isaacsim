Este exemplo independente fornece um script genérico para executar um exemplo de seguimento de alvo em qualquer robô compatível que use o RMPflow para alcançar um alvo enquanto evita obstáculos. O objetivo deste script é mostrar apenas como usar o RMPflow e, por uma questão de simplicidade, ele não usa o paradigma de tarefa/controlador típico em outros exemplos do Isaac Sim.

O script ./supported_robot_follow_target_example.py é executado com o caminho para o recurso USD do robô (que se presume estar armazenado no servidor Nucleus) e o nome do robô. Ao executar o script com os argumentos de linha de comando padrão, a lista de nomes de robôs compatíveis será impressa no terminal.

###### Argumentos da linha de comando

Os argumentos da linha de comando suportados são os seguintes:

-v,--verbose: Se True, imprime informações úteis de tempo de execução, como a lista de nomes de robôs suportados que mapeiam para arquivos de configuração RMPflow. O padrão é 'True'

    --robot-name: Nome do robô que mapeia para a configuração RMPflow armazenada.  O padrão é “Cobotta_Pro_900”

    --usd-path: Caminho para o ativo USD do robô no servidor Nucleus.  O padrão é “/Isaac/Robots/Denso/cobotta_pro_900.usd”.  A localização típica de um robô específico é em 
                “/Isaac/Robots/{nome_do_fabricante}/{nome_do_robô}/{nome_do_robô}.usd”

    --add-orientation-target: Adiciona a orientação do cubo alvo ao alvo RMPflow. O padrão é False.


###### Escolhendo o argumento correto para o nome do robô

Com os argumentos padrão, o script acima será executado usando o robô Cobotta Pro 900 e produzirá a seguinte saída:

    Nomes dos robôs compatíveis com a configuração RMPflow fornecida
        [‘Franka’, ‘UR3’, ‘UR3e’, ‘UR5’, ‘UR5e’, ‘UR10’, ‘UR10e’, ‘UR16e’, ‘Rizon4’, 'Cobotta_Pro_900', ‘Cobotta_Pro_1300’, ‘RS007L’, ‘RS007N’, ‘RS013N’, ‘RS025N’, ‘RS080N’, ‘FestoCobot’]

    Configuração RMPflow referenciada com sucesso para Cobotta_Pro_900.  Usando os seguintes parâmetros para inicializar a classe RmpFlow:
    {
        ‘end_effector_frame_name’: ‘gripper_center’,
        ‘ignore_robot_state_updates’: False,
        ‘maximum_substep_size’: 0.00334,
        'rmpflow_config_path': ‘/path/to/omni_isaac_sim/_build/linux-x86_64/release/exts/isaacsim.robot_motion.motion_generation/motion_policy_configs/./Denso/cobotta_pro_900/rmpflow/cobotta_rmpflow_common.yaml’,
        'robot_description_path': ‘/caminho/para/omni_isaac_sim/_build/linux-x86_64/release/exts/isaacsim.robot_motion.motion_generation/motion_policy_configs/./Denso/cobotta_pro_900/rmpflow/robot_descriptor.yaml’,
        'urdf_path': '/caminho/para/omni_isaac_sim/_build/linux-x86_64/release/exts/isaacsim.robot_motion.motion_generation/motion_policy_configs/./ Denso/cobotta_pro_900/rmpflow/../cobotta_pro_900_gripper_frame.urdf'
    }

Os nomes dos robôs compatíveis são adequados para o argumento `--robot-name`, e cada um deve corresponder corretamente ao caminho USD do robô.  Em uma versão futura, os dados de configuração para robôs compatíveis serão centralizados de forma que apenas um único argumento será necessário.  O método específico de acesso às configurações RMPflow dos robôs suportados fornecido aqui será então descontinuado.

A saída restante mostra as informações de configuração RMPflow encontradas sob o nome “Cobotta_Pro_900”.  Esta configuração é usada para inicializar a classe `RmpFlow`.


###### Exemplos de carregamento de outros robôs

Várias combinações válidas de argumentos de linha de comando são mostradas para diferentes robôs compatíveis:

python.sh supported_robot_follow_target_example.py --robot-name RS080N --usd-path “/Isaac/Robots/Kawasaki/RS080N/rs080n_onrobot_rg2.usd”

    python.sh supported_robot_follow_target_example.py --robot-name UR16e --usd-path “/Isaac/Robots/UniversalRobots/ur16e/ur16e.usd”

    python.sh supported_robot_follow_target_example.py --robot-name FestoCobot --usd-path “/Isaac/Robots/Festo/FestoCobot/festo_cobot.usd”
