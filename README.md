# WarTest

            <datasources>
                <datasource jta="true" jndi-name="java:jboss/datasources/BKFDS" pool-name="BKFDS" enabled="true" use-java-context="true" use-ccm="true">
                    <connection-url>jdbc:oracle:thin:@34.240.82.192:1521/JICSDV</connection-url>
                    <driver>oracle</driver>
                    <transaction-isolation>TRANSACTION_READ_COMMITTED</transaction-isolation>
                    <pool>
                        <min-pool-size>10</min-pool-size>
                        <max-pool-size>1000</max-pool-size>
                        <prefill>true</prefill>
                        <use-strict-min>true</use-strict-min>
                        <flush-strategy>FailingConnectionOnly</flush-strategy>
                    </pool>
                    <security>
                        <user-name>BKF</user-name>
                        <password>BKF</password>
                    </security>
                </datasource>
                <datasource jta="true" jndi-name="java:jboss/datasources/SSRDS" pool-name="SSRDS" enabled="true" use-java-context="true" use-ccm="true">
                    <connection-url>jdbc:oracle:thin:@34.240.82.192:1521/JICSDV</connection-url>
                    <driver>oracle</driver>
                    <transaction-isolation>TRANSACTION_READ_COMMITTED</transaction-isolation>
                    <pool>
                        <min-pool-size>10</min-pool-size>
                        <max-pool-size>1000</max-pool-size>
                        <prefill>true</prefill>
                        <use-strict-min>true</use-strict-min>
                        <flush-strategy>FailingConnectionOnly</flush-strategy>
                    </pool>
                    <security>
                        <user-name>SSR</user-name>
                        <password>SSR</password>
                    </security>
                </datasource>
                <drivers>
                    <driver name="oracle" module="com.oracle.ojdbc8">
                        <xa-datasource-class>oracle.jdbc.OracleDriver</xa-datasource-class>
                    </driver>
                </drivers>
            </datasources>
