# Definitions

## Overview

Zabbixの用語を示す。

## Definitions

### host

IP/DNSで表されるネットワークの監視対象。

### host group

ホストの論理グループ。ユーザグループごとにアクセス権を設定するときに使える。

### item

監視対象から受け取る情報・メトリクス

### value preprocessing

メトリックをデータベースに保存する前の処理。

### trigger

受け取ったデータを障害状態とみなすための閾値を表現するもの。  
データが閾値を上回ると "Problem" の状態となり、下回ると "Ok" になる。

### event

トリガーの状態の変化やタスクの自動実行などのできごとを表す。

### event tag

イベントに紐づけるタグ。事前に定義する。

### event correlation

問題と解決策を紐づける手段？  
あるトリガーにおけるある問題が別のトリガーによって解決される場合がある、といった関係性を定義できる？

### problem

"Problem" 状態のトリガー。

### problem update

problemにコメントをつけたり手動で解決状態にできる機能。

### action

イベントに反応する操作で、事前に定義するもの。  
operationsと conditionsからなる。

### escalation

アクションの内部で実行されるカスタムシナリオ。通知とかコマンド実行とか。

### media

通知を送ること。

### notification

指定の media channelに送られるイベントについてのメッセージ。

### remote command

条件に応じて監視対象のホストで自動的に実行されるコマンド。

### template

ホストに適用される item, trigger, graphなどの設定のまとまり。  
主に監視登録の高速化・簡略化を目的としたもの。

### template group

templateの論理グループ。ユーザごとに異なるアクセス権を付与するときに使う。

### web scerario

webサイトの可用性をチェックするためのリクエスト群。

### frontend

Zabbixの web GUI。

### dashboard

web GUIで表示できる情報のかたまり。ウィジェットの集まり？

### widget

dashboardの中に表示できる情報。

### Zabbix API

host, item, graphなどの情報の読み書きができる API。

### Zabbix server

Zabbixの中核となるプロセスで、監視の処理を担っている。triggerを計算したり、通知を送信したり。

### Zabbix proxy

Zabbix serverの代わりに情報を収集するもの。

### Zabbix agent

そのまんま。

### Zabbix agent 2

カスタムの監視ができる次世代のエージェント。

### encryption

TLSを使った通信の暗号化のこと。

### network discovery

そのまんま。

### low-level discovery

デバイスのインタフェース、ファイルシステムなどの自動検知。

### item prototype

low-level discoveryで使えるメトリックの変数。

### trigger prototype

low-level discoveryの変数として使えるトリガー。

### agent autoregistration

agentが自身を自動的に hostとして登録するプロセス。

